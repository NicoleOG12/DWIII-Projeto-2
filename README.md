# 📂 Projeto 2 — Processamento de Arquivos com Node.js e RegEx

## 🚀 Sobre o Projeto

Este projeto foi desenvolvido com o objetivo de aplicar conceitos fundamentais de **Node.js**, com foco na **manipulação de arquivos do sistema operacional** e na **extração de dados utilizando Expressões Regulares (RegEx)**.

O sistema lê um arquivo Markdown contendo referências técnicas e realiza a extração estruturada dos links presentes no documento.

---

## 🎯 Objetivo

Criar um script funcional capaz de:

* Ler um arquivo `.md` de forma assíncrona
* Identificar e extrair links em formato Markdown
* Organizar e exibir essas informações no console de forma clara e estruturada
* Tratar possíveis erros durante a execução

---

## 🧠 Tecnologias Utilizadas

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![fs](https://img.shields.io/badge/fs/promises-Node.js-blue?style=for-the-badge)
![path](https://img.shields.io/badge/path-Node.js-lightgrey?style=for-the-badge)
![RegEx](https://img.shields.io/badge/RegEx-Pattern-red?style=for-the-badge)
![Chalk](https://img.shields.io/badge/chalk-terminal-green?style=for-the-badge)
---

## 📁 Estrutura do Projeto

```
📦 projeto
 ┣ 📜 app.js
 ┣ 📜 package.json
 ┣ 📜 Projeto2_arquivo.md
 ┗ 📜 README.md
```

---

## ⚙️ Funcionalidades

### 📌 1. Leitura Assíncrona de Arquivo

Utiliza `fs/promises` com `async/await` para ler o arquivo sem bloquear a execução da aplicação.

---

### 📌 2. Extração com Expressão Regular

A seguinte RegEx é utilizada para capturar:

```
\[([^\]]*)\]\((https?:\/\/[^$#\s].[^\s]*)\)
```

Ela permite extrair:

* 📎 Nome da referência (texto entre colchetes)
* 🌐 URL (link entre parênteses)

---

### 📌 3. Tratamento de Erros

Caso o arquivo não seja encontrado ou ocorra algum problema:

* O erro é capturado com `try/catch`
* Uma mensagem destacada é exibida no terminal utilizando **chalk**

---

### 📌 4. Saída Formatada

Os dados extraídos são exibidos no console no seguinte formato:

```
Referência: Nome do Link | Link: https://exemplo.com
```

---

## ▶️ Como Executar o Projeto

### 1. Clone o repositório

```bash
git clone https://github.com/NicoleOG12/DWIII-Projeto-2.git
```

---

### 2. Acesse a pasta do projeto

```bash
cd DWIII-Projeto-2
```

---

### 3. Instale as dependências

```bash
npm install
```

---

### 4. Execute o projeto

```bash
node app.js
```

---

## 👩‍💻 Autora

**Nicole Oliveira Gonçalves**
