<h2 align="center">Robert Kennedy</h2>
<h4 align="center">Backend Developer · Go · APIs REST · PostgreSQL · Docker</h4>

<p align="center">
  <a href="https://www.linkedin.com/in/robert-kennedy-034687369/">
    <img src="https://img.shields.io/badge/LinkedIn-Conectar-0A66C2?style=flat&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:robert_unix@hotmail.com">
    <img src="https://img.shields.io/badge/Email-Contato-D44638?style=flat&logo=gmail&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/Disponível-Remoto%20%7C%20Júnior-1D9E75?style=flat" />
  <img src="https://img.shields.io/badge/Manaus-AM%2C%20Brasil-555?style=flat" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Echo-Framework-00ACD7?style=flat&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/REST-API-6BA539?style=flat" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white" />
</p>

---

Desenvolvo backends em Go com foco em **APIs REST**, **arquitetura modular** e **sistemas que precisam funcionar sob pressão**.

Antes de migrar para desenvolvimento, trabalhei em ambientes de tecnologia de alta criticidade — setor militar e central de operações (CIOPS/AM) — onde sistemas que falham têm consequências reais. Esse background moldou meu jeito de escrever código: com atenção à resiliência, segurança e performance desde o início.

---

## Projetos

### 🛒 [go-api-vitrine](https://github.com/robert-kennedy-devops/go-api-vitrine) — API REST CRUD em Go
> Projeto de referência para recrutadores: código limpo, testado e documentado.

```
Stack  →  Go 1.21 · Echo v4 · PostgreSQL 16 · Docker
Testes →  22 testes unitários · race detector limpo · sem dependência de banco
```

**Destaques técnicos:**
- Arquitetura em 3 camadas: `handler` → `service` → `repository`
- Repository pattern com interface — troca de storage (memória ↔ PostgreSQL) sem alterar o resto
- PATCH parcial com ponteiros (`*string`, `*float64`) para distinguir campo ausente de zero value
- Build multi-stage Docker: imagem final ~5MB em Alpine, sem código-fonte

```bash
git clone https://github.com/robert-kennedy-devops/go-api-vitrine
go run ./cmd/api   # sobe em segundos, sem banco necessário
```

---

### ⚔️ [tormenta-rpg-bot](https://github.com/robert-kennedy-devops/tormenta-rpg-bot) — MMORPG multiplayer no Telegram
> Sistema de backend complexo, projetado para escalar até 1 milhão de usuários.

```
Stack  →  Go · PostgreSQL · Docker · Telegram Bot API
Schema →  21 migrações SQL incrementais
```

**Destaques técnicos:**
- Engine de combate desacoplada (`internal/engine/`) — sem efeitos colaterais, testável isoladamente
- Event bus assíncrono com pool de 8 goroutines e fila de 10k slots
- Camada de segurança dedicada: rate limiting por ação, dedup de callbacks, detecção de bot-pattern
- Workers de background concorrentes: combate, economia, raids, eventos

---

### 🤖 [KeroBot](https://github.com/robert-kennedy-devops/KeroBot) — Cliente MTProto Telegram
> Integração com protocolo MTProto nativo — nível abaixo da Bot API padrão.

```
Stack  →  Go · gotd/td · PostgreSQL · Docker
```

**Destaques técnicos:**
- Protocolo MTProto via `gotd/td` — acesso direto à API do Telegram
- Arquitetura event-driven com separação `pkg/` (público) e `internal/` (privado)
- Logs estruturados · CHANGELOG versionado · Licença MIT

---

## Stack

| | Tecnologia |
|---|---|
| Linguagem | Go (Golang) |
| APIs | RESTful · Echo Framework · Telegram Bot API · MTProto |
| Banco de dados | PostgreSQL · SQL puro · migrations versionadas |
| DevOps | Docker · Docker Compose · Linux |
| Práticas | Repository pattern · injeção de dependência · testes unitários · race detector |

---

## Background

Anos em ambientes onde indisponibilidade não é opção:

- **Exército Brasileiro** (2006–2007) — infraestrutura de missão crítica, zero tolerância a falhas
- **CIOPS/AM** (2010) — monitoramento em tempo real, resposta a incidentes de alta prioridade
- **Slake Infor** (2017–hoje) — gestão de servidores Linux em produção, redes, troubleshooting avançado

---

<p align="center">
  <i>Aberto a oportunidades Backend Júnior · 100% remoto · Manaus, AM</i><br>
  <a href="https://www.linkedin.com/in/robert-kennedy-034687369/">linkedin.com/in/robert-kennedy-034687369</a>
</p>
