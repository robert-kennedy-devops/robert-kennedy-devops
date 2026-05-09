<h2 align="center">Robert Kennedy</h2>
<h4 align="center">Backend Developer · Go · SaaS · APIs REST · PostgreSQL · Docker</h4>

<p align="center">
  <a href="https://www.linkedin.com/in/robert-kennedy-034687369/">
    <img src="https://img.shields.io/badge/LinkedIn-Conectar-0A66C2?style=flat&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:robert_unix@hotmail.com">
    <img src="https://img.shields.io/badge/Email-Contato-D44638?style=flat&logo=gmail&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/Disponível-Remoto%20%7C%20Backend%20Júnior-1D9E75?style=flat" />
  <img src="https://img.shields.io/badge/Manaus-AM%2C%20Brasil-555?style=flat" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/REST-API-6BA539?style=flat" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white" />
</p>

---

Desenvolvo backends em Go com foco em **APIs REST**, **SaaS**, **arquitetura modular**, **integrações externas** e **sistemas concorrentes**.

Antes de migrar para desenvolvimento, trabalhei em ambientes de tecnologia de alta criticidade — setor militar, central de operações e administração de servidores Linux — onde indisponibilidade, falhas de segurança e falta de observabilidade têm impacto real. Esse background moldou meu jeito de escrever software: simples de operar, seguro por padrão e preparado para crescer.

---

## Projetos em destaque

### 🟢 [SlakeZAPI](https://github.com/robert-kennedy-devops/SlakeZAPI) — Plataforma SaaS para WhatsApp
> SaaS multi-tenant em Go para envio, recebimento e operação de mensagens WhatsApp, com dashboard em Next.js e integração real via WhatsMeow.

```
Stack  →  Go · PostgreSQL · Docker · Next.js · WhatsMeow · Stripe
Escopo →  API REST · WebSocket · Webhooks · Billing · Dashboard · Multi-instância
```

**Destaques técnicos:**
- Clean Architecture com separação entre domínio, use cases, repositórios, transporte HTTP e integrações externas
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

```
Stack  →  Go · PostgreSQL · Docker · Telegram Bot API · AbacatePay
Schema →  21 migrações SQL incrementais
Escopo →  RPG · PvP · Guildas · Economia · Raids · Temporadas · Pagamentos Pix
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

```
Stack  →  Go 1.21 · Echo v4 · PostgreSQL 16 · Docker
Escopo →  CRUD REST · Repository Pattern · Testes · Storage in-memory/PostgreSQL
```

**Destaques técnicos:**
- Arquitetura em camadas: `handler` → `service` → `repository`
- Repository pattern com interface para alternar entre storage in-memory e PostgreSQL
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
| Frontend de produto | Next.js · dashboard SaaS · autenticação de usuário |
| Mensageria e integrações | WhatsMeow · Telegram Bot API · Webhooks · WebSocket |
| Billing e pagamentos | Stripe · AbacatePay/Pix · webhooks de pagamento |
| DevOps | Docker · Docker Compose · Linux · health checks |
| Segurança | API keys com hash · bcrypt · HMAC · rate limiting · proteção SSRF · CORS |
| Observabilidade | Logs estruturados · métricas Prometheus · readiness/liveness · filas e DLQ |
| Testes | Testes unitários · race detector · código desacoplado por interfaces |

---

## Background

Experiência prática em ambientes onde indisponibilidade não é opção:

- **Exército Brasileiro** (2006–2007) — infraestrutura de missão crítica e disciplina operacional
- **CIOPS/AM** (2010) — monitoramento em tempo real e resposta a incidentes de alta prioridade
- **Slake Infor** (2017–hoje) — administração de servidores Linux em produção, redes e troubleshooting avançado

---

## Foco atual

- Desenvolvimento backend em Go
- APIs REST e produtos SaaS
- Sistemas multi-tenant
- PostgreSQL, Docker e Linux
- Integrações com WhatsApp, Telegram, Webhooks e Billing
- Código simples de operar, seguro e testável

---

<p align="center">
  <i>Aberto a oportunidades Backend Júnior · 100% remoto · Manaus, AM</i><br>
  <a href="https://www.linkedin.com/in/robert-kennedy-034687369/">linkedin.com/in/robert-kennedy-034687369</a>
</p>
