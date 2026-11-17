<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/signal-cartography-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/signal-cartography-light.svg">
  <img src="./assets/signal-cartography-light.svg" alt="Banner vetorial com meu nome, grade geométrica e linhas de sinal inspiradas em engenharia e música." width="100%">
</picture>

# Kelwin Feitosa

**Desenvolvimento de software · IA aplicada à engenharia · Automações · MusicTech**

Trabalho com **desenvolvimento de software, inteligência artificial e automações**. Nos projetos de engenharia, estudo APIs, modelagem e qualidade; em experimentos pessoais, exploro como agentes de IA podem transformar requisitos em implementações, e quais são os limites dessa abordagem.

Combino **Java e Spring Boot**, **Python** e interesse em computação musical. Distingo código publicamente verificável, protótipos conduzidos com IA e funcionalidades ainda não homologadas.

**Brasília, Brasil** · Ciência da Computação na **UDF** (conclusão prevista para dez/2027) · Interesse em **estágios, vagas júnior e colaboração remota**, inclusive internacional.

[**Código público**](#projetos-em-destaque) · [**Experimentos com IA**](#experimentos-com-ia) · [LinkedIn](https://www.linkedin.com/in/kelwinfeitosa/) · [E-mail](mailto:kelwinfeitosa@gmail.com) · [**Read in English**](./README.en.md)

---

## Projetos em destaque

**Código público:** os repositórios abaixo permitem examinar implementações, arquitetura, documentação e testes diretamente.

### 01 · [Supermarket Management API](https://github.com/kelwin-feitosa/supermarket-management-api)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/case-systems-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/case-systems-light.svg">
  <img src="./assets/case-systems-light.svg" alt="Esquema decorativo representando módulos de catálogo, estoque e vendas." width="100%">
</picture>

**Java 21 · Spring Boot 4 · PostgreSQL · Spring Security · Docker**

API para operações de supermercado, incluindo catálogo, fornecedores, estoque, compras, carrinhos e vendas.

- **Engenharia:** monólito modular por domínio, validação, operações transacionais, autenticação com JWT e consultas com filtros e paginação.
- **Evidências:** testes automatizados com JUnit e Mockito, documentação da API e integração contínua com GitHub Actions.
- **Estado real:** backend em evolução; interface administrativa e frente de caixa permanecem planejadas.

[**Ver código, arquitetura e testes**](https://github.com/kelwin-feitosa/supermarket-management-api#readme)

### 02 · [Assistente Financeiro com IA](https://github.com/kelwin-feitosa/assistente-financeiro)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/case-ai-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/case-ai-light.svg">
  <img src="./assets/case-ai-light.svg" alt="Esquema decorativo de fluxo de voz, modelo de IA, ferramentas e serviços de domínio." width="100%">
</picture>

**Java 21 · Spring Boot · Spring AI · MySQL · Gemini**

API de transações financeiras com solicitações em linguagem natural, desenvolvida como projeto final do **bootcamp Itaú / DIO — Java com Inteligência Artificial**.

- **Engenharia:** *tool calling* encaminha operações para serviços da aplicação, mantendo a integração com IA separada das regras de negócio.
- **Recursos:** criação e consulta de transações, transcrição local com Whisper.cpp e síntese de voz com Piper.
- **Evidências:** testes com JUnit/Mockito e pipeline de CI com MySQL. A interpretação de linguagem natural utiliza serviço externo.

[**Explorar implementação e limitações**](https://github.com/kelwin-feitosa/assistente-financeiro#readme)

<details>
<summary><strong>Outros trabalhos públicos e fundamentos</strong></summary>

- [**Simulador de empréstimo (Java SE)**](https://github.com/kelwin-feitosa/simulador-emprestimo-java) — regras de análise de crédito, orientação a objetos e cálculos com `BigDecimal`; persistência em PostgreSQL ainda planejada.
- [**Projetos acadêmicos — UDF**](https://github.com/kelwin-feitosa/UDF-Projetos) — exemplos de desenvolvimento mobile, prototipação de interfaces e fundamentos de grafos.
- [**Exercism**](https://github.com/kelwin-feitosa/exercism) — prática de fundamentos e resolução de exercícios em Java.

</details>

## Experimentos com IA

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/case-ai-lab-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/case-ai-lab-light.svg">
  <img src="./assets/case-ai-lab-light.svg" alt="Ilustração de um ciclo conceitual de experimentação com IA: problema, especificação, geração, revisão e aprendizagem." width="100%">
</picture>

Estes três projetos são **experimentos pessoais de desenvolvimento fortemente assistido por IA**: usei modelos para gerar e evoluir grande parte das implementações, enquanto explorava definição de requisitos, direcionamento das iterações e avaliação dos resultados. Meu objetivo foi testar o **processo de trabalhar com IA no desenvolvimento**, não demonstrar autoria manual de cada módulo.

A existência de testes automatizados não significa que todos os fluxos tenham sido validados por mim em uso real. **Os códigos ainda estão em repositórios privados**, sujeitos a revisão antes de eventual publicação.

### 03 · FluteOMR — computação musical

**Python · processamento de imagens · MusicXML · protótipo experimental**

- **Experimento:** orientar a evolução de um reconhecedor óptico de partituras com regras musicais, corpus e avaliação técnica.
- **Estado documentado:** detecção de pautas, componentes de reconhecimento controlado, exportação MusicXML experimental e verificações automatizadas.
- **Limite:** ainda não reconhece partituras completas com precisão musical geral comprovada; referências reais e revisão humana continuam limitadas.

### 04 · Kelwin Hub — produtividade e automações locais

**Python · FastAPI · SQLite · interface web · piloto local**

- **Experimento:** investigar o desenvolvimento assistido por IA de um produto com vários módulos e critérios de privacidade e manutenção.
- **Estado documentado:** projetos, tarefas, contatos, oportunidades, agenda, alertas locais, autenticação e backup criptografado.
- **Limite:** não é produto homologado; integrações externas e envio automático de mensagens não fazem parte do escopo validado.

### 05 · Aurora — integração e automação acadêmica

**TypeScript · PWA · Gmail/Outlook · protótipo pré-homologação**

- **Experimento:** projetar com auxílio de IA um fluxo de identificação de compromissos em e-mails, com revisão humana e políticas de privacidade.
- **Estado documentado:** integração por provedores em código, sincronização e notificações previstas nos fluxos, interface instalável e testes com serviços simulados.
- **Limite:** OAuth com contas reais, implantação e entrega de notificações ainda exigem homologação; não é confiável como única fonte de prazos.

**Critério para divulgar código:** segurança, direitos de terceiros e descrição honesta do estágio — não a conclusão de todas as funcionalidades.

## Engenharia na prática

| Área | Tecnologias e práticas presentes nos projetos |
| --- | --- |
| **Backend e domínio** | Java, Spring Boot, APIs REST, Spring Data JPA, Hibernate e validação |
| **Dados** | PostgreSQL, MySQL, modelagem relacional e Flyway |
| **Confiabilidade e segurança** | Spring Security, JWT, transações, tratamento de erros e revisão de limites |
| **Testes e entrega** | JUnit 5, Mockito, Maven, Docker, GitHub Actions e OpenAPI |
| **IA no desenvolvimento** | Especificação, iteração com agentes, análise crítica das saídas e experimentação assistida |
| **Automações e MusicTech** | Python, fluxos locais, integração experimental, MusicXML e ferramentas musicais |

Procuro entender **por que** uma decisão técnica funciona. Em desenvolvimento com IA, isso também significa revisar saídas dos agentes, reconhecer o que não foi testado e separar evidências de hipóteses — em vez de tratar código gerado como automaticamente correto.

## Música e computação

Sou formado em **flauta transversal pela Escola de Música de Brasília**. Essa experiência orienta as perguntas que exploro em computação musical: leitura de partituras, **MusicXML**, reconhecimento óptico e educação musical. O **FluteOMR** é um experimento nessa interseção.

## Contato

Tenho interesse em colaborar com equipes de **desenvolvimento, IA aplicada, automação, backend e MusicTech**, em oportunidades de início de carreira.

**[LinkedIn](https://www.linkedin.com/in/kelwinfeitosa/)** · **[E-mail](mailto:kelwinfeitosa@gmail.com)** · **[Todos os repositórios públicos](https://github.com/kelwin-feitosa?tab=repositories)**

<sub>Projetos públicos e experimentos assistidos por IA são identificados separadamente. Nenhum experimento privado é apresentado como software homologado. O conteúdo essencial permanece acessível sem imagens ou animações.</sub>
