# Olá, eu sou o Kelwin👋

Desenvolvedor em formação focado no ecossistema **Java**. Priorizo código limpo, lógica bem estruturada e a construção de arquiteturas modulares. Atualmente no 5º semestre de Ciência da Computação.

## 🛠️ Stack Técnica
- **Linguagem:** Java (JDK 21)
- **Framework:** Spring Boot
- **Banco de Dados:** PostgreSQL (JDBC)
- **SO:** Pop!_OS (Linux) | **IDE:** VS Code

## 🏗️ Projetos em Destaque

### [MA7H_31GMA5 (Math Enigmas)](LINK_DO_REPOSITORIO)
API REST para gestão de sessões de desafios matemáticos.
- **Funcionamento:** O sistema utiliza `records` para transferência de dados (DTOs) e gerencia o estado da rodada em memória via UUIDs, validando a resposta do cliente sem expô-la no payload.
- **Lógica:** Implementa um serviço de sorteio baseado em níveis de dificuldade (`enum`), filtrando questões de um catálogo JSON através de Stream API.
- **Tratamento de Erros:** Centralizado em um `GlobalExceptionHandler` que intercepta exceções de negócio e falhas de desserialização JSON.

### [Simulador de Empréstimo Bancário](LINK_DO_REPOSITORIO)
Sistema de análise de crédito focado em integridade financeira e persistência de dados.
- **Lógica de Negócio:** Separação clara de responsabilidades entre `EmprestimoService` e `ValidadorEmprestimo`, utilizando `BigDecimal` com `RoundingMode.HALF_UP` para cálculos monetários precisos.
- **Infraestrutura:** Implementação de uma `FabricaConexao` robusta que utiliza arquivos de propriedades externos (`.properties`) e o driver JDBC para comunicação com o **PostgreSQL**.
- **Robustez:** Sistema de exceções personalizadas (`NegocioException`) e testes de conectividade integrados para validar a integração com o banco de dados.

## 📫 Contato:
- **LinkedIn:** [kelwinfeitosa](https://www.linkedin.com/in/kelwinfeitosa)
- **E-mail:** kelwinfeitosa@gmail.com

<div style="display: inline_block">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" width="40" height="40" alt="Java" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg" width="40" height="40" alt="Spring" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" width="40" height="40" alt="Postgres" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" width="40" height="40" alt="Linux" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="40" height="40" alt="VSCode" />
</div>
