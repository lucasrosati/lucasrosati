# Lucas Rosati

**Engineering with LLMs, not just prompting them.**

### What I'm working on

- **SitecomAI** · AI Engineer. Multi-provider AI stack with capability-based routing, provider health monitoring, cost tracking and deterministic CI replay, plus agent runtimes and CI infrastructure for autonomous coding.
- **MedFoco** · Founder/CTO. SaaS for Brazilian medical education: AI-generated study content for students from P1 to P12 (React, PostgreSQL, Claude API).
- **GNI · Global News Intelligence** · CTO. Predictive intelligence platform: multi-source news monitoring, scenario forecasting, risk boards and automated intelligence reports.
- **Argos** · Agentic-first personal ERP. Agents operate it through a remote MCP server; tasks close themselves on PR merge.
- **FORGE** · Co-founder.

### What I'm into

- Multi-agent orchestration: subagents, git worktrees, parallel Claude Code and Codex CLI sessions
- Persistent memory for coding agents (Obsidian Zettelkasten as long-term context)
- Context engineering: AST-derived codebase knowledge graphs (Graphify) as an alternative to embedding-based RAG
- Model routing and cost optimization across providers
- Automation pipelines that turn manual workflows into systems

### Open source

- [claude-code-memory-setup](https://github.com/lucasrosati/claude-code-memory-setup) · 1k stars · Persistent memory and codebase knowledge graphs for Claude Code (Obsidian + Graphify). Cuts tokens per session by up to 71.5x. EN and PT-BR docs.
- [agent-throttle](https://github.com/lucasrosati/agent-throttle) · Run several coding agents on one machine without taking it down: worker ceilings enforced by hooks, memory checks and tuning metrics.
- [greenlight](https://github.com/lucasrosati/greenlight) · Serial task queue for headless Claude Code. Nothing merges without a human.
- [claude-security-agents](https://github.com/lucasrosati/claude-security-agents) · Red Team and Blue Team agents for Claude Code that automate security audits.
- [claude-maestro](https://github.com/lucasrosati/claude-maestro) · Parallel Claude Code agents via tmux, single script, no frameworks.

### Hit me up

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-rosati-cavalcanti-pereira-b62229128)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/lucasrosati)
[![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discordapp.com/users/lucasrosati)
[![Email](https://img.shields.io/badge/Email-0078D4?style=for-the-badge&logo=microsoftoutlook&logoColor=white)](mailto:lucasrosati@hotmail.com)

## Tech Stack

![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0DB7ED?style=for-the-badge&logo=docker&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-191919?style=for-the-badge&logo=anthropic&logoColor=D97757)

**AI & LLM Systems**
- Claude API (Batch, Structured Outputs), OpenAI, Gemini, Deepgram, OpenRouter
- Model gateway: capability-based routing, provider fallback, health checks, per-call cost ledger
- Model tiering by task: Haiku triage, Sonnet editorial, Opus orchestration
- RAG with hybrid retrieval and grounded citations (pgvector, embeddings routed through the gateway)
- Schema-gated LLM output: Pydantic, JSON Schema, defensive JSON extraction that fails loud
- Voice AI: real-time STT → LLM → TTS over WebSockets
- Deterministic replay of LLM calls in CI

**Agent Platforms**
- Isolated Claude Code runners with egress boundaries, lifecycle gates and session memory
- Autonomous queues for headless Claude Code: SHA-bound CI gates, review babysitting, nothing merges without a human
- Remote MCP servers with bearer auth, built so agents operate the system as first-class users
- Multi-agent orchestration: git worktrees, Orca, Claude Code + Codex CLI in parallel, per-machine resource throttling
- Persistent agent memory: Obsidian Zettelkasten, session hooks, cross-agent handoffs
- Context engineering: AST-derived codebase knowledge graphs (Graphify), up to 71.5x fewer tokens per session

**Backend & Distributed Systems**
- Python: FastAPI, SQLAlchemy 2, Alembic, Pydantic v2, asyncio, Dramatiq, APScheduler
- TypeScript: NestJS, Prisma, Socket.IO, Node.js workers
- Event-driven integration hubs: canonical models, anti-corruption layers, outbox pattern, idempotent consumers
- Multi-tenant architecture: Postgres RLS, RBAC, immutable audit trail with hash chain
- Execution state machines and cost ledgers with exact decimal money
- Integrations: JIRA, Stripe, Telegram, WhatsApp (Evolution API), Google Ads/Analytics APIs, GitHub webhooks (HMAC), OFX bank statements, S3

**Data**
- PostgreSQL 16/17 (partitioning, RLS, advisory locks, triggers), pgvector, Redis, SQLite
- Ingestion pipelines: RSS and Telegram feeds, dedup and fuzzy clustering, legacy content migration
- Headless CMS on Postgres (Payload + Next.js)

**Infra & DevOps**
- Docker, Docker Compose, GHCR images, Caddy, Cloudflare
- GCP Cloud Run, DigitalOcean, Linux, systemd
- GitHub Actions: required checks, ruleset drift detection, agent-driven fix runners
- Observability: OpenTelemetry, Prometheus, Sentry
- Release safety: snapshot before deploy, rollback runbooks, backups off the host

**Testing & Quality**
- pytest, Hypothesis (property-based), pytest-randomly, Vitest, Maestro (mobile E2E)
- ruff, mypy, Biome, pip-audit
- E2E tests against real databases

**Frontend & Mobile**
- React, TypeScript, Vite, TanStack Query/Router, Tailwind
- React Native + Expo
- Next.js
