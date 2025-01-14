# 🧵 Fórum Hub API

Este projeto é uma **API RESTful** desenvolvida para o gerenciamento de tópicos e discussões. Ele foi criado como parte do desafio promovido pela **Alura**, em parceria com o programa **Oracle Next Education**.

---

## 🚀 Tecnologias Utilizadas

- **Linguagem:** Java 17
- **Framework:** Spring Boot (v3.3.5)
- **Banco de Dados:** MySQL, com migrações gerenciadas via Flyway
- **Gerenciamento de Dependências:** Maven
- **Validação e Segurança:** Spring Validation e Spring Security
- **Autenticação:** JWT (Java Web Token)
- **Documentação:** Gerada automaticamente com Springdoc OpenAPI

---

## 📦 Principais Dependências

A configuração completa está disponível no arquivo **`pom.xml`**, mas as principais dependências incluem:

- **Spring Boot Starter Web:** Desenvolvimento de APIs REST.
- **Spring Boot Starter Data JPA:** Manipulação de dados no banco de dados.
- **Spring Boot Starter Validation:** Validação de dados de entrada.
- **Spring Boot Starter Security:** Configuração de autenticação e autorização.
- **Flyway:** Migração e versionamento do banco de dados.
- **Lombok:** Redução de código boilerplate.
- **Springdoc OpenAPI:** Geração de documentação interativa.
- **MySQL Connector:** Conexão com o banco de dados MySQL.

---

## ✨ Funcionalidades

### 🔹 Cadastro de Tópicos
- Criação de novos tópicos, com validação de título e mensagem.

### 🔹 Listagem de Tópicos
- Visualização dos tópicos registrados, com suporte a paginação e ordenação.

### 🔹 Detalhamento de Tópico
- Exibição detalhada de informações de um tópico pelo ID.

### 🔹 Atualização e Exclusão
- Atualização de informações existentes.
- Exclusão lógica, marcando os tópicos como inativos.

### 🔹 Autenticação JWT
- Acesso seguro, garantindo que apenas usuários autenticados possam acessar endpoints protegidos.

---

## 🛠️ Testes com Insomnia

É recomendado o uso do **Insomnia** para testar os endpoints da API. Configure variáveis de ambiente para simplificar as requisições e inclua o token JWT para autenticar os endpoints protegidos.

---

### 🗂️ Estrutura do Projeto

Organização das pastas no projeto para fácil navegação e manutenção:

```plaintext
src/
├── main/
│   ├── java/
│   │   ├── com.example.forumhub/
│   │   │   ├── controllers/
│   │   │   ├── services/
│   │   │   ├── repositories/
│   │   │   ├── models/
│   │   │   └── configs/
│   └── resources/
│       ├── application.properties
│       └── db/
│           └── migration/
└── test/
    └── java/
