# Esta é uma revisão com intutito de reforçar os conceitos aprendido no curso...

# Spring Boot E-commerce API

Este repositório contém um exemplo de API de comércio eletrônico desenvolvida com Spring Boot. A aplicação inclui funcionalidades básicas de CRUD para usuários, produtos, pedidos, categorias e itens de pedidos.

## Visão Geral

A API oferece os seguintes recursos:

- **Usuários**
- **Produtos**
- **Categorias**
- **Pedidos**
- **Itens de Pedido**
- **Pagamentos**

Cada recurso está implementado com camadas de controle, serviço e repositório, além de uma camada de tratamento de exceções.

## Estrutura do Projeto

- **Entities:** Contém as classes que representam as tabelas do banco de dados.
- **Repositories:** Interfaces que extendem `JpaRepository` para operações de CRUD.
- **Services:** Contêm a lógica de negócios da aplicação.
- **Resources:** Contêm os controladores REST que expõem os endpoints da API.
- **Exceptions:** Contêm as classes de exceções customizadas e o handler global de exceções.

## Endpoints

### Usuários

- `GET /users` - Retorna todos os usuários.
- `GET /users/{id}` - Retorna um usuário por ID.
- `POST /users` - Cria um novo usuário.
- `PUT /users/{id}` - Atualiza um usuário existente.
- `DELETE /users/{id}` - Deleta um usuário.

### Produtos

- `GET /products` - Retorna todos os produtos.
- `GET /products/{id}` - Retorna um produto por ID.
- `POST /products` - Cria um novo produto.
- `PUT /products/{id}` - Atualiza um produto existente.
- `DELETE /products/{id}` - Deleta um produto.

### Categorias

- `GET /categories` - Retorna todas as categorias.
- `GET /categories/{id}` - Retorna uma categoria por ID.
- `POST /categories` - Cria uma nova categoria.
- `PUT /categories/{id}` - Atualiza uma categoria existente.
- `DELETE /categories/{id}` - Deleta uma categoria.

### Pedidos

- `GET /orders` - Retorna todos os pedidos.
- `GET /orders/{id}` - Retorna um pedido por ID.
- `POST /orders` - Cria um novo pedido.
- `PUT /orders/{id}` - Atualiza um pedido existente.
- `DELETE /orders/{id}` - Deleta um pedido.

## Exceções

A API lida com as seguintes exceções:

- **ResourceNotFoundException:** Lançada quando um recurso não é encontrado.
- **DatabaseException:** Lançada quando ocorre um erro de banco de dados.

## Configuração e Execução

### Pré-requisitos

- Java 11 ou superior
- Maven 3.6 ou superior
- Banco de dados H2 (ou outro banco de dados de sua escolha)

