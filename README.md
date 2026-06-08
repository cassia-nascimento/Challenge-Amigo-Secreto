<h1 align="center">
   🎁 Challenge Amigo Secreto — Oracle Next Education (ONE)
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Alura-ONE-Orange?style=for-the-badge" alt="Alura ONE">
</p>

Repositório dedicado à resolução do **Challenge Amigo Secreto**, o primeiro desafio prático de desenvolvimento de software proposto pela trilha inicial de lógica de programação do programa **Oracle Next Education (ONE)**, realizado em parceria com a **Alura**.

A aplicação simula um gerenciador reativo de sorteios onde os usuários podem inserir uma lista de participantes e realizar a escolha aleatória de um "amigo secreto" de forma automatizada.

<p align="center">
  <img src="assets/tela-inicial.png" alt="Tela Inicial do Projeto Amigo Secreto" width="85%">
</p>

---

## 📌 Regras de Negócio & Engenharia de Lógica

O motor do sistema (estruturado puramente em `app.js`) foi arquitetado para tratar erros de entrada de dados e gerenciar o estado da interface visual através das seguintes operações:

* **Validação de Entrada Estrita:** Impede a inserção de strings vazias ou espaços em branco na lista. Caso o usuário tente clicar no botão de adicionar sem preencher o campo, o sistema dispara um alerta nativo de aviso.
* **Manipulação de Arrays (Persistência em Memória):** Cada nome válido é capturado via DOM, inserido em um array dinâmico (`amigos`) e o input de texto é limpo imediatamente para otimizar a usabilidade.
* **Renderização Dinâmica de Elementos HTML:** Uma função iteradora percorre o array a cada atualização, limpa o nó anterior do DOM e cria novos elementos de lista (`<li>`) injetados diretamente na tag correspondente, exibindo os nomes cadastrados em tempo real.
* **Algoritmo de Sorteio Aleatório:** Utilizando funções matemáticas nativas (`Math.random()` combinado com `Math.floor()`), o sistema sorteia um índice baseado no tamanho atual da lista. Uma validação prévia garante que o sorteio só ocorra se houver participantes cadastrados.

<p align="center">
  <img src="assets/adicionar.png" alt="Fluxo de Cadastro" width="49%">
  <img src="assets/detalhamento.png" alt="Detalhamento" width="49%">
</p>

---

## 📂 Organização dos Arquivos

```text
challenge-amigo-secreto
├── assets/             # Componentes de design, ícones e ilustrações da interface
├── app.js              # Camada lógica pura (orquestração do DOM, arrays e sorteio)
├── index.html          # Marcação estrutural e semântica do layout
└── style.css           # Tokens visuais, tipografias e estilização responsiva

```

---

## 🚀 Como Executar o Projeto

Por se tratar de uma aplicação front-end client-side pura, ela roda de forma nativa no navegador sem necessidade de ferramentas de terminal ou servidores backend:

1. Realize o clone deste repositório em sua máquina:
```bash
git clone https://github.com/cassia-nascimento/challenge-amigo-secreto.git

```


2. Acesse a pasta do projeto:
```bash
cd challenge-amigo-secreto

```


3. Abra o arquivo `index.html` diretamente em qualquer navegador web de sua preferência (Chrome, Firefox, Safari ou Edge).

---

## 👩‍💻 Autora

Desafio construído e documentado com foco em boas práticas por **Cássia Nascimento**.

* [GitHub Profile](https://github.com/cassia-nascimento)
* [LinkedIn](https://www.linkedin.com/in/cassia--nascimento/)
