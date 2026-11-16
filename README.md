# 👶 Chá do Rayan - Sistema de RSVP

Um aplicativo web elegante, rápido e de arquivo único (Single-Page) desenvolvido para gerenciar confirmações de presença (RSVP) para um Chá de Bebê. 

O sistema permite que os convidados confirmem presença facilmente e oferece uma área restrita para os organizadores visualizarem e gerenciarem a lista de convidados em tempo real.

## ✨ Funcionalidades

* **Formulário Simples:** Os convidados podem confirmar se irão ou não, e adicionar os nomes de seus acompanhantes.
* **Área Restrita (Lista de Convidados):** Uma aba protegida por senha onde os organizadores podem ver todos que confirmaram.
* **Contadores Automáticos:** Painel que soma automaticamente o total de confirmados (incluindo acompanhantes) e o total de pessoas que não poderão ir.
* **Gerenciamento em Tempo Real:** Conectado ao Firebase Firestore, a lista é atualizada instantaneamente e permite excluir nomes de testes/desistências diretamente pela interface.
* **Design Responsivo e Moderno:** Interface desenhada com Tailwind CSS, perfeitamente adaptada para celulares e computadores.

## 🛠️ Tecnologias Utilizadas

Este projeto foi construído de forma simplificada utilizando CDNs, o que significa que **não requer instalação de pacotes (npm)** e roda diretamente no navegador:

* **HTML5**
* **React.js** (via CDN)
* **Tailwind CSS** (via CDN para estilização)
* **Babel** (Standalone via CDN para compilar JSX no navegador)
* **Firebase** (Firestore Database para armazenamento em nuvem)

## 🚀 Como Utilizar e Hospedar

Como o projeto é um arquivo HTML único, colocá-lo no ar é extremamente simples:

1. **Clone ou Baixe o projeto:**
   Faça o download do arquivo `index.html`.

2. **Configure o Banco de Dados (Firebase):**
   * Crie um projeto gratuito no [Firebase](https://console.firebase.google.com/).
   * Crie um banco de dados **Firestore** e inicie no "Modo de Teste" (ou configure as Regras para `allow read, write: if true;`).
   * Adicione um "App Web" no Firebase e copie as chaves de configuração.
   * Cole as suas chaves no arquivo `index.html` na variável `firebaseConfig`.

3. **Hospede Gratuitamente (Deploy):**
   * Faça o upload do arquivo `index.html` para um repositório público no GitHub.
   * Vá nas **Settings** (Configurações) do repositório > **Pages**.
   * Em *Source*, selecione a branch `main` e salve. 
   * Em poucos minutos, seu site estará no ar através do link gerado pelo GitHub Pages!

## 🔒 Acesso à Lista de Convidados

Para acessar a aba "Lista de Convidados" no site rodando, utilize a seguinte senha padrão:
* **Senha:** `1234`
*(Você pode alterar esta senha diretamente na linha `if (passwordInput === '1234')` dentro do arquivo `index.html`).*

---
*Desenvolvido com carinho para celebrar momentos especiais.* 🍼
