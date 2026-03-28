# Digital Store - Backend

API backend de uma aplicação de e-commerce digital, responsável pelo gerenciamento de produtos e carrinhos de compra.

---

## Sobre o Projeto

Este projeto consiste em uma API REST desenvolvida para simular o funcionamento de uma loja virtual de produtos digitais. A aplicação permite operações completas de CRUD para produtos e gerenciamento de carrinhos de compra.

O objetivo principal é praticar conceitos de desenvolvimento backend, organização de rotas e manipulação de dados.

---

## Tecnologias Utilizadas

- Node.js
- Express.js
- JavaScript
- JSON (armazenamento de dados)

---

## Funcionalidades

### Produtos
- Listar todos os produtos
- Buscar produto por ID
- Criar novos produtos
- Atualizar produtos existentes
- Remover produtos

---

### Carrinho de Compras
- Criar carrinho
- Buscar carrinho por ID
- Adicionar produtos ao carrinho

---

### Produtos

| Método | Rota | Descrição |
|------|------|----------|
| GET | /api/products | Lista todos os produtos |
| GET | /api/products/:id | Retorna um produto específico |
| POST | /api/products | Cria um novo produto |
| PUT | /api/products/:id | Atualiza um produto |
| DELETE | /api/products/:id | Remove um produto |

---

### Carrinho

| Método | Rota | Descrição |
|------|------|----------|
| POST | /api/carts | Cria um carrinho |
| GET | /api/carts/:id | Retorna um carrinho |
| POST | /api/carts/:cid/products/:pid | Adiciona produto ao carrinho |

---

## Conceitos Aplicados

- Estruturação de API REST
- CRUD completo
- Organização de rotas
- Separação de responsabilidades
- Manipulação de dados em memória (JSON)
- Boas práticas com Express

---

## Estrutura do Projeto

src/
├── routes/
├── controllers/
├── services/
├── data/
└── app.js


---

## Como Executar o Projeto
```bash
1. Clone o repositório
git clone https://github.com/raphimw2e/digital-store-backend.git

2. Acesse a pasta
cd digital-store-backend

3. Instale as dependências
3.1. npm install
3.2. npm install express
3.3. npm install dotenv
3.4. npm install sequelize
3.5. npm install jsonwebtoken
3.6. npm install bcryptjs
3.7. npm install cors
3.8. npm install --save-dev nodemon sequelize-cli
3.9. npm install swagger-jsdoc swagger-ui-express

4. Execute o servidor
npm start
```

### Testando a API
Você pode testar os endpoints utilizando:
- Postman
- Insomnia

O projeto inclui coleções prontas para facilitar os testes.

### Melhorias Futuras

- Autenticação de usuários
- Validação de dados
- Upload de imagens
- Sistema de pagamentos
- Deploy em nuvem

### Licença
Este projeto está sob a licença MIT.

--- 
### Autora

Desenvolvido por Rafaela Araújo 

---
### 1. Badges no topo
```md
![Node.js](https://img.shields.io/badge/Node.js-18-green)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)
``` 

### 2. Exemplo de JSON de resposta

{
  "id": 1,
  "name": "Produto Exemplo",
  "price": 29.90
}
