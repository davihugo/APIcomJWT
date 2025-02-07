# API REST com JWT e Swagger

API REST desenvolvida com Spring Boot 3.2.2, utilizando JWT para autenticação e Swagger para documentação.

## 🚀 Tecnologias

- Java 17
- Spring Boot 3.2.2
- Spring Security
- JWT (JSON Web Token)
- Swagger (OpenAPI 3)
- H2 Database
- Maven

## 📋 Pré-requisitos

- Java 17 ou superior
- Maven

## 🔧 Instalação

1. Clone o repositório:
2. Execute o projeto:
bash
mvn spring-boot:run


## 📚 Documentação da API

Após iniciar a aplicação, acesse a documentação Swagger em: http://localhost:8080/swagger-ui.html


## 🔒 Endpoints

### Autenticação

#### Registro de Usuário
bash
POST /auth/register
Content-Type: application/json
{
"username": "seu_usuario",
"password": "sua_senha"
}

#### Login
bash
POST /auth/login
Content-Type: application/json
{
"username": "seu_usuario",
"password": "sua_senha"
}

O endpoint de login retorna um token JWT que deve ser incluído no header `Authorization` das requisições subsequentes:
Authorization: Bearer seu_token_jwt


## 🔐 Segurança

- Autenticação stateless usando JWT
- Senha criptografada usando BCrypt
- CORS configurado
- Endpoints protegidos por Spring Security

## 📝 Configurações

As principais configurações estão no arquivo `application.properties`:

- Banco de dados H2
- Chave secreta JWT
- Configurações do Swagger
- Configurações de CORS



