# 👋 Olá, eu sou o Kelwin!

🎓 **Estudante de Ciência da Computação**  
💻 **Desenvolvedor Backend em formação**  
☕ **Java | Spring Boot | PostgreSQL**

Sou estudante de Ciência da Computação e desenvolvedor backend em formação, com foco no ecossistema Java e no desenvolvimento de APIs REST.

Gosto de transformar problemas em soluções através de código, buscando desenvolver aplicações organizadas, testáveis e alinhadas às boas práticas de desenvolvimento.

Atualmente, estou aprofundando meus conhecimentos em **Java, Spring Boot, bancos de dados, testes, segurança e arquitetura de software**, enquanto busco uma oportunidade de estágio para aplicar meus conhecimentos em um ambiente profissional.

---

## 🚀 Sobre mim

```java
public class Kelwin {

    String curso = "Ciência da Computação";
    String foco = "Desenvolvimento Backend";

    String[] principaisTecnologias = {
        "Java",
        "Spring Boot",
        "Spring Data JPA",
        "Hibernate",
        "PostgreSQL"
    };

    String[] praticas = {
        "APIs REST",
        "Testes automatizados",
        "Docker",
        "CI/CD",
        "Segurança com JWT"
    };

    String objetivo =
        "Tornar-me um desenvolvedor backend cada vez melhor";
}
```

---

## 🛠️ Stack

### ☕ Backend

![Java](https://img.shields.io/badge/Java-21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring%20Data%20JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)

### 🔐 Segurança

![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![BCrypt](https://img.shields.io/badge/BCrypt-Password%20Hashing-59666C?style=for-the-badge)

### 🗄️ Banco de Dados

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-17-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![H2](https://img.shields.io/badge/H2-Database-09476B?style=for-the-badge)

### 🧪 Testes e Qualidade

![JUnit](https://img.shields.io/badge/JUnit%205-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![Mockito](https://img.shields.io/badge/Mockito-78A641?style=for-the-badge)
![JaCoCo](https://img.shields.io/badge/JaCoCo-Coverage-EF2D5E?style=for-the-badge)
![SonarCloud](https://img.shields.io/badge/SonarCloud-F3702A?style=for-the-badge&logo=sonarcloud&logoColor=white)

### 🐳 Ferramentas e DevOps

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker%20Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

---

# 🚀 Projeto em Destaque

## 🛒 Supermarket Management API

API REST desenvolvida com **Java 21** e **Spring Boot 4** para simular o backend de um sistema de gerenciamento de supermercado.

O projeto aplica conceitos utilizados em aplicações backend, incluindo **arquitetura em camadas, persistência relacional, regras de negócio, segurança, testes automatizados, documentação, migrações de banco de dados, containerização e integração contínua**.

### ✨ Funcionalidades

- 🛍️ CRUD de produtos
- 🏷️ CRUD de categorias
- 👤 Gerenciamento de usuários
- 🏭 Gerenciamento de fornecedores
- 📦 Controle de estoque
- 🛒 Carrinho de compras
- ➕ Adição e alteração de itens
- ➖ Remoção de itens
- 🧮 Cálculo automático de subtotais
- 💰 Cálculo do valor total
- 🧾 Conversão de carrinho em venda
- 📊 Histórico de vendas
- 📉 Baixa automática de estoque
- ✅ Validação de disponibilidade
- 🔎 Filtros dinâmicos com JPA Specifications
- 📄 Paginação de resultados
- ⚠️ Tratamento global de exceções
- 📋 Validação com Jakarta Validation
- 🔐 Autenticação com JWT
- 🔑 Hash de senhas com BCrypt
- 🛡️ Autorização baseada em roles
- 📚 Documentação com Swagger / OpenAPI
- 🧪 Testes com JUnit 5 e Mockito
- 📈 Cobertura de código com JaCoCo
- 🔎 Análise de qualidade com SonarCloud
- 🗄️ Migrações de banco com Flyway
- 🐳 PostgreSQL executado com Docker Compose
- 🔄 Integração contínua com GitHub Actions

### 🏗️ Arquitetura

```text
src
├── main
│   ├── java
│   │   └── com.exemplo.meu_primeiro_projeto
│   │       ├── config
│   │       ├── controller
│   │       ├── dto
│   │       │   ├── filter
│   │       │   ├── request
│   │       │   └── response
│   │       ├── exception
│   │       ├── mapper
│   │       ├── model
│   │       ├── repository
│   │       │   └── specification
│   │       ├── security
│   │       │   ├── filter
│   │       │   └── service
│   │       ├── service
│   │       └── util
│   │
│   └── resources
│       ├── db
│       │   └── migration
│       └── application.properties
│
└── test
    ├── java
    └── resources
        └── application-test.properties
```

### 🔐 Segurança

A API utiliza **Spring Security**, **JWT** e **BCrypt**.

A autenticação é stateless e utiliza tokens JWT enviados através do header:

```http
Authorization: Bearer <token>
```

O controle de acesso utiliza diferentes roles e `@PreAuthorize`:

```text
SYSTEM_ADMIN
      ↓
   MANAGER
    ↙   ↘
STOCK_MANAGER  CASHIER

CUSTOMER
```

A chave utilizada para assinar os tokens JWT é fornecida através da variável de ambiente `JWT_SECRET`.

### 🧰 Tecnologias

```text
Java 21
Spring Boot 4
Spring Security
Spring Data JPA
Hibernate
Jakarta Validation
JWT
BCrypt
PostgreSQL
Flyway
JUnit 5
Mockito
JaCoCo
Swagger / OpenAPI
Docker
Docker Compose
Maven
Git
GitHub Actions
SonarCloud
```

### 🔗 Repositório

[![GitHub](https://img.shields.io/badge/GitHub-Supermarket%20Management%20API-181717?style=for-the-badge&logo=github)](https://github.com/kelwin-feitosa/supermarket-management-api)

---

# 💰 Outro Projeto

## Simulador de Empréstimos Bancários

Aplicação Java desenvolvida para simular empréstimos bancários, com foco em **precisão matemática, persistência de dados e organização da lógica de negócio**.

### Principais conceitos

- `BigDecimal`
- `RoundingMode.HALF_UP`
- JDBC
- PostgreSQL
- Validação de dados
- Exceções personalizadas
- Separação de responsabilidades

[![GitHub](https://img.shields.io/badge/GitHub-Simulador%20de%20Empréstimos-181717?style=for-the-badge&logo=github)](https://github.com/kelwin-feitosa/simulador-emprestimo-java)

---

# 📚 Atualmente estudando

- Testes de integração
- Testcontainers
- Concorrência
- Arquitetura de Software
- Microsserviços
- Cloud
- Integração com Inteligência Artificial

---

## 📊 GitHub

<div align="center">

<img src="./profile/stats.svg" height="180em"/>

<img src="./profile/top-langs.svg" height="180em"/>

</div>

---

## 🐍 Contribuições

<div align="center">

<img
  src="https://raw.githubusercontent.com/kelwin-feitosa/kelwin-feitosa/gh-pages/github-contribution-grid-snake-dark.svg"
  alt="GitHub Contribution Snake"
/>

</div>

---

# 📫 Onde me encontrar

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kelwin%20Feitosa-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kelwinfeitosa)

[![Email](https://img.shields.io/badge/Email-kelwinfeitosa%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kelwinfeitosa@gmail.com)

</div>

---

<div align="center">

### ☕ Transformando café em código.

</div>
