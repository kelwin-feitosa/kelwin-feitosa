# 👋 Olá, eu sou o Kelwin!

🎓 **Estudante de Ciência da Computação**  
💻 **Desenvolvedor Backend em formação**  
☕ **Java | Spring Boot | PostgreSQL**

Sou estudante de Ciência da Computação e desenvolvedor backend em formação, com foco no ecossistema Java e no desenvolvimento de APIs REST.

Gosto de transformar problemas em soluções através de código, buscando escrever aplicações organizadas, testáveis e próximas das práticas utilizadas no desenvolvimento profissional.

Atualmente, estou focado em evoluir como desenvolvedor backend e busco uma oportunidade de estágio para colocar meus conhecimentos em prática.

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
        "CI/CD"
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

O projeto aplica conceitos utilizados em aplicações backend reais, incluindo arquitetura em camadas, persistência relacional, validação, tratamento de exceções, testes automatizados, documentação, migrações de banco de dados, containerização e integração contínua.

### ✨ Funcionalidades

- 🛍️ CRUD de produtos
- 🏷️ CRUD de categorias
- 👤 Gerenciamento de clientes
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
│   │       ├── exception
│   │       ├── mapper
│   │       ├── model
│   │       ├── repository
│   │       │   └── specification
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

### 🧰 Tecnologias

```text
Java 21
Spring Boot 4
Spring Data JPA
Hibernate
Jakarta Validation
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

Aplicação Java desenvolvida para simular empréstimos bancários, com foco em precisão matemática e organização da lógica de negócio.

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

- Spring Security
- JWT
- BCrypt
- Testes de integração
- Testcontainers
- Concorrência
- Microsserviços
- Arquitetura de Software
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
