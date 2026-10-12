# Toggle Master Microservices - Observabilidade



## **Identificação do Projeto**

- **Projeto:** Toggle Master Microservices
- **Fase:** 04 - Observabilidade
- **Integrantes:** Grupo 68
  - Arthur de Castilho Nascimento - RM371601 - [castartx@gmail.com](mailto:castartx@gmail.com)
  - Gerusa Fernandes Lobo Nogueira - RM367568 - [gerusalobo@gmail.com](mailto:gerusalobo@gmail.com)
  - José Henrique Cavalcanti de Melo Filho -  RM 372074 - [meloricke.bra@gmail.com](mailto:meloricke.bra@gmail.com)
  - Pedro Vinicius Araujo Negreiros - RM372553 - [pedro28vinicius@hotmail.com](mailto:pedro28vinicius@hotmail.com)


## Objetivo do Projeto

A arquitetura é dividida nos em 5 microsserviços:

auth-service (Go): Gerencia chaves de API e autenticação. (Banco de Dados: PostgreSQL)

flag-service (Python): CRUD das definições das feature flags. (Banco de Dados: PostgreSQL)

targeting-service (Python): Gerencia regras complexas de segmentação. (Banco de Dados: PostgreSQL)

evaluation-service (Go): O "caminho quente" (hot path) de alta performance que retorna a decisão final (true/false). (Cache: Redis)

analytics-service (Python): Consome eventos de uma fila e salva dados de análise. (Fila: AWS SQS, Banco de Dados: AWS DynamoDB)

A missão desse projeto é implementar toda a parte de observabilidade nos microserviços de forma a monitorar e gerar alertas das aplicações.


## Arquitetura
