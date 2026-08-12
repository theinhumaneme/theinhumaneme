# Kalyan Mudumby

MSCS @ Northeastern University (Boston) • I build AI-powered apps and the platforms that keep them fast and reliable.

- Built **SMART AI Chat**, a public-facing LLM 311 assistant for the City of Fort Wayne, on LangChain + the OpenAI API
- Cut cold-start latency **100×** (20s → 200ms) with Redis pipelining, and page load **5×** (30s → 7s) with Brotli/Gzip and a 60% smaller bundle
- Reproducible CI/CD with Docker multi-stage builds on GitLab CI across **40+ services**
- Rust-first tooling for deployment automation and developer workflows

**Looking for:** summer 2027 internship / co-op roles in **AI/ML** or **platform engineering**.

**Links:** [Blog](https://kalyanmudumby.com) • [Resume](https://kalyanmudumby.com/kalyan_mudumby_resume.pdf) • [LinkedIn](https://linkedin.com/in/kalyan-mudumby) • [Email](mailto:mudumby.k@northeastern.edu)

---

## Stack
- **Languages:** Rust, Python, TypeScript/JavaScript, Java, SQL, Bash
- **App/AI:** LangChain, LangGraph, Google ADK, MCP, FastAPI, Flask, Spring Boot, Angular, React, Postgres, Redis, WebSockets
- **Infra/DevOps:** Linux, Docker, GitLab CI, Nginx, Cloudflare, OpenTelemetry, Prometheus/Grafana, Kubernetes, NixOS

---

## Featured projects

- **[Hikari](https://github.com/theinhumaneme/hikari)** — GitOps platform in async Rust, a lightweight Kubernetes alternative for small VM fleets
  Rust + Tokio + Axum + Postgres/SQLx • WebSocket agent/server design for real-time config propagation
  Each agent reconciles its host against the last-applied declarative JSON config; AES-256-CBC config secrets under an RSA-4096 OAEP envelope. Nine tagged releases.
  Write-ups: [Agent/server design](https://kalyanmudumby.com/post/scale-vm-management-with-hikari-agent-server/) • [Daemon mode](https://kalyanmudumby.com/post/rule-vms-with-hikari/)

- **[Patternsmith](https://github.com/theinhumaneme/patternsmith)** — multi-agent LLM pipeline that turns a topic into a publication-ready tutorial
  Python + LangGraph + Pydantic v2 + Hugo • Research/Teaching → Code → Writing → validation over one typed state
  Generated code is embedded verbatim, so it never drifts from the prose or the Mermaid diagrams. Model-agnostic behind a ChatLLM protocol: the same pipeline runs against a hosted API or a local model (Ollama / LM Studio) on one config flag. MIT licensed.
  Site: [patternsmith.distroy.dev](https://patternsmith.distroy.dev)

- **[Documan](https://github.com/theinhumaneme/documan-public-release)** — a college digital library where every subject has an address: department, year, semester
  Ran in production on Flask/Postgres for five years (Jun 2020 – May 2025): 4,000+ students, 200,000+ file deliveries, 1,200+ active users, 99%+ uptime, over a web app and a Telegram bot.
  Then rewrote it from scratch as a Java 25 / Spring Boot 4.1 API (virtual threads, Redis caching, Cloudflare R2, Meilisearch kept in step with Postgres by a transactional outbox) plus an Angular 21 signals client, identity on Clerk. The rewrite has no users; it is where the interesting engineering is.
  Write-up: [Zero-cost digital library](https://kalyanmudumby.com/post/documan-zero-cost-digital-library/)

- **[Autodeploy](https://github.com/theinhumaneme/autodeploy)** — single Rust binary that turns a TOML config into a working local deployment
  Interactive CLI (git2, inquire) that generates Docker Compose at runtime for multi-service stacks. Cut local environment setup from an estimated 2 hours to 20 minutes.
  Write-up: [Hassle-free deployments](https://kalyanmudumby.com/post/hasslefree-deployments-with-autodeploy/)

---

## Open source

- **LangChain [#19427](https://github.com/langchain-ai/langchain/pull/19427)** — fixed a Pydantic serialization bug in the GPTCache integration, where a `ChatGeneration` returned by `ChatOpenAI` was not handled on cache lookup. Merged Mar 2024.

---

## Awards

- **Best Podman Container Implementation** and **People's Choice** — Pods, Prompts & Prototypes Hackathon (Red Hat / IBM), Mar 2026, for OAAM (Open Agent Applet Marketplace): a local-first AI web app that extracts structured data from documents fully on-device via RamaLama + Podman AI Lab.
- **Star of the Month** — Nebulogic Technologies, May 2024.

---

## Writing

- Observability for modern workloads: metrics, logs, tracing
- DNS privacy and running your own resolver stack
- Deployment automation lessons from Hikari and Autodeploy

Read here: [Blog home](https://kalyanmudumby.com)
