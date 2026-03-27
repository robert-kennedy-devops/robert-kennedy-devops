<h1 align="center">Robert Kennedy</h1>
<h3 align="center">Backend Developer · Go · APIs REST · Docker · PostgreSQL</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/robert-kennedy-034687369/">
    <img src="https://img.shields.io/badge/LinkedIn-robert--kennedy-0A66C2?style=flat&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:robert_unix@hotmail.com">
    <img src="https://img.shields.io/badge/Email-robert__unix%40hotmail.com-D44638?style=flat&logo=gmail&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/Localização-Manaus%2C%20AM-green?style=flat" />
  <img src="https://img.shields.io/badge/Disponível-Remoto-1D9E75?style=flat" />
</p>

---

## Sobre mim

Desenvolvedor Backend com foco em **Go**, construindo sistemas que precisam ser rápidos, confiáveis e escaláveis.

Antes de migrar para desenvolvimento, passei anos em ambientes de tecnologia de alta criticidade — setor militar e central de operações (CIOPS/AM) — onde aprendi que sistemas que falham têm consequências reais. Isso moldou meu jeito de escrever código: com atenção à resiliência, segurança e performance desde o início.

Hoje aplico esse background no desenvolvimento de **backends em Go**, com arquitetura modular, APIs REST bem definidas e deploy containerizado.

---

## Stack

```
Linguagem      Go (Golang)
APIs           RESTful · Echo Framework · Telegram Bot API (MTProto)
Banco de dados PostgreSQL · modelagem relacional · migrations SQL
DevOps         Docker · Docker Compose · Linux (administração avançada)
Práticas       Arquitetura modular · Clean Code · variáveis de ambiente · .gitignore correto
```

---

## Projetos em destaque

### ⚔️ [tormenta-rpg-bot](https://github.com/robert-kennedy-devops/tormenta-rpg-bot)
> MMORPG multiplayer para Telegram — arquitetura projetada para escalar até 1 milhão de usuários

**Stack:** Go · PostgreSQL · Docker · Telegram Bot API

**Destaques técnicos:**
- Engine de combate modular (`internal/engine/`) com interfaces bem definidas, sem efeitos colaterais
- Sistema de segurança dedicado (`internal/security/`) com rate limiting por ação, deduplicação de callbacks/transações, detecção de comportamento anômalo e logger JSON estruturado
- Event bus com pool de goroutines e fila de 10k slots para comunicação assíncrona entre subsistemas
- 21 migrações SQL incrementais com schema versionado
- Workers de background (combate, economia, eventos, raids) com concorrência controlada
- Camada de cache unificada com fallback mem → Redis

---

### 🤖 [KeroBot](https://github.com/robert-kennedy-devops/KeroBot)
> Cliente de usuário Telegram (MTProto) com automação de ações em estilo RPG

**Stack:** Go · gotd/td · PostgreSQL · Docker

**Destaques técnicos:**
- Protocolo MTProto via `gotd/td` — nível mais baixo que a Bot API padrão
- Arquitetura event-driven com separação entre `pkg/` (público/reutilizável) e `internal/`
- Logs estruturados e configuração via `.env`
- Licença MIT · CHANGELOG versionado

---

## Background que trago para o código

| Experiência | Aplicação no desenvolvimento |
|---|---|
| Exército Brasileiro — Setor de Informática (2006–2007) | Disciplina operacional, sistemas sem tolerância a falhas |
| CIOPS/AM — Monitoramento em tempo real (2010–2011) | Análise de incidentes, resposta rápida, logs e rastreabilidade |
| 8+ anos como Técnico de TI (Slake Infor) | Infraestrutura, redes, Linux, diagnóstico de sistemas |

---

## Em evolução contínua

- Testes em Go (unitários e de integração)
- gRPC e comunicação entre microserviços
- Redis para cache distribuído
- Observabilidade (métricas, tracing)

---

<p align="center">
  <i>Aberto a oportunidades de Backend Júnior — 100% remoto · Manaus, AM</i>
</p>
