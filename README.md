<h1 align="center">Robert Kennedy</h1>

<h3 align="center">Backend Developer. · Go · APIs REST · PostgreSQL · Docker · Linux</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/robert-kennedy-034687369/">
    <img src="https://img.shields.io/badge/LinkedIn-Conectar-0A66C2?style=flat&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:robert_unix@email.com">
    <img src="https://img.shields.io/badge/Email-robert__unix%40email.com-D44638?style=flat&logo=gmail&logoColor=white" />
  </a>
  <a href="https://github.com/robert-kennedy-devops">
    <img src="https://img.shields.io/badge/GitHub-robert--kennedy--devops-181717?style=flat&logo=github&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/Disponível-Backend%20Júnior%20%7C%20Remoto-1D9E75?style=flat" />
  <img src="https://img.shields.io/badge/Manaus-AM%2C%20Brasil-555?style=flat" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/REST-API-6BA539?style=flat" />
  <img src="https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=flat&logo=swagger&logoColor=black" />
</p>

---

## Sobre mim

Sou desenvolvedor backend em formação profissional, com foco em **Go**, **APIs REST**, **PostgreSQL**, **Docker**, **Linux** e construção de sistemas simples de operar, seguros e testáveis.

Antes de focar em desenvolvimento de software, atuei em ambientes de tecnologia onde disponibilidade, segurança e resposta a incidentes importam de verdade: administração de servidores Linux, redes, troubleshooting, operação técnica e suporte a ambientes críticos. Esse histórico influencia meu estilo de engenharia: prefiro soluções objetivas, observáveis, documentadas e preparadas para manutenção.

Atualmente busco oportunidades como **Backend Developer**, com foco em:

```text
Go · APIs REST · PostgreSQL · Docker · Linux · Testes · Cloud básico
```

---

## Projeto de estudo estruturado

### 📘 [E-book: Backend Júnior com Go](https://github.com/robert-kennedy-devops/Backend-junior-com-go) — Roadmap de portfólio backend

Projeto/roadmap técnico para consolidar fundamentos de backend júnior usando Go.

```text
Stack  → Go · PostgreSQL · Docker · JWT · Redis · Swagger/OpenAPI · Testes · Cloud
Escopo → API REST · Auth · CRUD · Migrations · Arquitetura em camadas · Deploy
```

# E-book: Backend Júnior com Go

Material de estudo em formato de e-book para quem deseja iniciar ou consolidar fundamentos de desenvolvimento backend usando **Go**, **APIs REST**, **PostgreSQL**, **Docker**, **testes**, **documentação técnica** e **cloud básico**.

Este repositório existe para distribuição do e-book e como material complementar de portfólio.

## Sobre o e-book

**Título:** Backend Júnior com Golang, PostgreSQL, Docker, APIs e Cloud  
**Autor:** Robert Kennedy  
**Formato:** PDF  
**Público-alvo:** iniciantes em desenvolvimento backend, estudantes de programação e pessoas em transição para primeira vaga júnior.

## Objetivo

Apresentar uma trilha prática e didática para estudar backend com Go, cobrindo desde conceitos básicos de programação até tópicos usados em projetos reais.

O conteúdo aborda:

- fundamentos de desenvolvimento backend;
- introdução à linguagem Go;
- variáveis, tipos, funções, structs, interfaces e tratamento de erros;
- controle de fluxo com `if`, `else`, `switch` e `for`;
- HTTP, REST e JSON;
- PostgreSQL e SQL;
- migrations;
- arquitetura em camadas;
- autenticação com JWT;
- Docker e Docker Compose;
- testes unitários e de integração;
- Swagger/OpenAPI;
- Redis, cache e filas;
- logs e observabilidade;
- deploy em cloud;
- projeto final de portfólio;
- glossário de siglas;
- roteiro de entrevista técnica.

---

## Projetos em destaque

### 🟢 [SlakeZAPI](https://github.com/robert-kennedy-devops/SlakeZAPI) — Plataforma SaaS para WhatsApp

> SaaS multi-tenant em Go para envio, recebimento e operação de mensagens WhatsApp, com dashboard em Next.js e integração real via WhatsMeow.

```text
Stack  → Go · PostgreSQL · Docker · Next.js · WhatsMeow · Stripe
Escopo → API REST · WebSocket · Webhooks · Billing · Dashboard · Multi-instância
```

**Destaques técnicos:**

- Clean Architecture com separação entre domínio, casos de uso, repositórios, transporte HTTP e integrações externas
- Multi-tenancy com tenants, usuários, memberships, API keys e múltiplas instâncias WhatsApp
- Dashboard SaaS em Next.js com autenticação, inbox operacional, campanhas, webhooks, billing e gestão de conta
- Integração WhatsApp avançada: texto, mídia, grupos, status, contatos, localização, stickers, reações, edição e encaminhamento
- Sessões seguras com refresh token em cookie `HttpOnly`, access token em memória e suporte a WebSocket em tempo real
- Billing autosserviço com Stripe: checkout, upgrade/downgrade, portal de cobrança, webhook e planos mensais
- Segurança aplicada: hash de API keys, bcrypt, HMAC em webhooks, proteção SSRF, rate limit, CORS configurável e limites de payload
- Observabilidade com health checks, readiness/liveness, métricas Prometheus, fila observável e dead-letter queue

```bash
git clone https://github.com/robert-kennedy-devops/SlakeZAPI.git
cd SlakeZAPI
cp .env.example .env
docker compose --env-file .env -f docker/docker-compose.yml up --build -d
```

---

### ⚔️ [tormenta-rpg-bot](https://github.com/robert-kennedy-devops/tormenta-rpg-bot) — MMORPG multiplayer no Telegram

> Backend de jogo multiplayer em Go, inspirado em Tormenta 20, com arquitetura modular e foco em escalabilidade.

```text
Stack  → Go · PostgreSQL · Docker · Telegram Bot API · AbacatePay
Schema → 21 migrações SQL incrementais
Escopo → RPG · PvP · Guildas · Economia · Raids · Temporadas · Pagamentos Pix
```

**Destaques técnicos:**

- Engine de combate desacoplada em `internal/engine/`, testável isoladamente e sem efeitos colaterais
- Event bus assíncrono com pool fixo de goroutines e fila de 10k slots
- Segurança dedicada: rate limiting por ação, deduplicação de callbacks, anti-exploit e detecção de comportamento anômalo
- Workers de background para combate, economia, eventos e raids
- Cache em camadas com interface para Redis e fallback in-memory
- Conteúdo RPG gerado programaticamente: classes, raças, habilidades, itens, monstros, combos e progressão

```bash
git clone https://github.com/robert-kennedy-devops/tormenta-rpg-bot.git
cd tormenta-rpg-bot
cp .env.example .env
docker compose up -d
```

---

### 🛒 [go-api-vitrine](https://github.com/robert-kennedy-devops/go-api-vitrine) — API REST CRUD em Go

> Projeto de referência para demonstrar fundamentos sólidos de backend: organização de código, testes unitários, Docker e PostgreSQL.

```text
Stack  → Go 1.21 · Echo v4 · PostgreSQL 16 · Docker
Escopo → CRUD REST · Repository Pattern · Testes · Storage in-memory/PostgreSQL
```

**Destaques técnicos:**

- Arquitetura em camadas: `handler` → `service` → `repository`
- Repository Pattern com interface para alternar entre storage in-memory e PostgreSQL
- PATCH parcial com ponteiros para diferenciar campo ausente de zero value
- Testes unitários de service e repository, incluindo cenário concorrente com race detector
- Execução rápida sem banco: se `DATABASE_URL` não estiver definido, a API sobe em memória

```bash
git clone https://github.com/robert-kennedy-devops/go-api-vitrine.git
cd go-api-vitrine
go run ./cmd/api
```

---

## Stack principal

| Área | Tecnologias e práticas |
|---|---|
| Linguagem | Go (Golang) |
| Backend | APIs REST · Clean Architecture · Repository Pattern · Injeção de dependência manual |
| Banco de dados | PostgreSQL · SQL puro · migrações versionadas |
| Containers | Docker · Docker Compose |
| Sistema operacional | Linux · administração de servidores · troubleshooting |
| Frontend de produto | Next.js · dashboard SaaS · autenticação de usuário |
| Mensageria e integrações | WhatsMeow · Telegram Bot API · Webhooks · WebSocket |
| Billing e pagamentos | Stripe · AbacatePay/Pix · webhooks de pagamento |
| Segurança | API keys com hash · bcrypt · HMAC · rate limiting · proteção SSRF · CORS |
| Observabilidade | Logs estruturados · métricas Prometheus · readiness/liveness · filas e DLQ |
| Testes | Testes unitários · testes de integração · race detector · código desacoplado por interfaces |
| Cloud/DevOps | Deploy básico · health checks · variáveis de ambiente · operação com Docker |

---

## Base técnica em evolução

Atualmente estou consolidando uma trilha focada em primeira vaga backend:

```text
1. Go para APIs REST
2. PostgreSQL e SQL
3. Docker e Docker Compose
4. Autenticação JWT
5. Testes unitários e integração
6. Swagger/OpenAPI
7. Redis e cache
8. Deploy em cloud
9. Observabilidade básica
```

---

## Background operacional

Experiência prática em ambientes onde indisponibilidade e falhas operacionais causam impacto real:

- **Exército Brasileiro** (2006–2007) — infraestrutura de missão crítica e disciplina operacional
- **CIOPS/AM** (2010) — monitoramento em tempo real e resposta a incidentes de alta prioridade
- **Slake Infor** (2017–hoje) — administração de servidores Linux em produção, redes e troubleshooting avançado

---

## Como avalio qualidade em backend

Para mim, um backend bem construído precisa ser:

```text
simples de rodar
fácil de testar
bem documentado
seguro por padrão
observável
separado em responsabilidades claras
preparado para evolução
```

---


<p align="center">
  <b>Aberto a oportunidades Backend Júnior · Remoto · Manaus, AM</b><br><br>
  <a href="https://www.linkedin.com/in/robert-kennedy-034687369/">LinkedIn</a> ·
  <a href="https://github.com/robert-kennedy-devops">GitHub</a> ·
  <a href="mailto:robert_unix@email.com">robert_unix@email.com</a>
</p>
