<h1 align="center">Hi, I'm Muhammad Asif 👋</h1>

<p align="center">
  <b>Software Engineer | Full-Stack Developer</b>
  <br />
  React.js · Next.js · Node.js · NestJS
</p>

<p align="center">
  <a href="mailto:asif.jsdev@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://linkedin.com/in/asif-jsdev">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <img src="https://img.shields.io/badge/Open%20to%20work-2ea44f?style=for-the-badge" alt="Open to work" />
</p>

Full-stack engineer, four years, mostly TypeScript. Most of that work has been on systems that already existed — replacing polling with WebSockets, indexing slow queries found by profiling, rewriting live APIs without changing behaviour for the people using them.

I also run two of my own projects in production, where the CI/CD, the server and the certificates are mine to fix when they break.

Open to full-stack and backend engineering roles — remote or Lahore.

<br />

## 📂 Projects

### 🗂️ &nbsp;[Job Tracker](https://github.com/muhammadasif2017/job-tracker) · [Live demo](https://job-tracker-blush-two.vercel.app)

An application for tracking job applications through each stage of a search. I built it because I needed one, and I use it daily.

- JWT access/refresh auth plus Google and GitHub OAuth2, using a server-side code exchange so tokens never appear in redirect URLs
- Company enrichment pulled from external services through an async BullMQ pipeline with retries and failure handling
- Runs in production on Oracle Cloud. Pull-based CI/CD, Jest and Playwright e2e tests against a live database

<sub>**NestJS** · PostgreSQL · Prisma · Next.js 16 · React 19 · TypeScript · BullMQ · Docker</sub>

### 💳 &nbsp;[Stripe Payment Sync](https://github.com/muhammadasif2017/stripe-payment-sync)

A NestJS backend that keeps orders, payments and refunds in step with Stripe, so no payment is lost or recorded twice, even when Stripe sends an event twice or the database goes down.

- Verified webhooks stored once by event ID, processed by a BullMQ worker with retries, and a daily reconciliation against Stripe that repairs anything missed
- Race conditions between the worker and reconciliation fixed test-first; hardened after a security review (rate limits, CSP, customer details kept out of stored events)
- 186 unit and 126 e2e tests; CI starts the whole stack in Docker and scans the image with Trivy. Includes a recorded end-to-end demo

<sub>**NestJS** · TypeScript · PostgreSQL · Prisma · Redis · BullMQ · Stripe · Docker · GitHub Actions</sub>

### 🔐 &nbsp;[Nest Nexus](https://github.com/muhammadasif2017/nest-nexus)

A NestJS backend that implements 6 different ways of signing in, each one properly. Most auth examples stop at a JWT and a login form, so I wanted a reference that went further.

- JWT with refresh-token rotation, OAuth2, TOTP 2FA, magic links, WebAuthn passkeys, API keys
- Token-family reuse detection on rotation, with atomic revoke-then-issue sequencing to block replay
- 17+ architecture decision records in the repo, if you want the reasoning behind any of it

<sub>**NestJS** · TypeScript · PostgreSQL · Prisma · Redis · BullMQ · Docker · Caddy</sub>

### 🤖 &nbsp;[Helpdesk Copilot](https://github.com/muhammadasif2017/helpdesk-copilot)

A helpdesk app with an LLM support assistant embedded in it — an LLM feature inside a real product, not a standalone chatbot.

- RAG over a knowledge base with cited sources, streamed into the ticket UI, refusing to invent policy it can't find
- Guardrails in the tools rather than the prompt: a state-changing action is proposed for human approval, and the tool re-verifies identity itself before acting
- Two-tier eval suite. Runs fully offline on Ollama, no external services

<sub>**Python** · FastAPI · SQLite + sqlite-vec · fastembed · Ollama</sub>

<br />

## 💼 Experience

- **Afiniti** · Software Engineer · 2024–2025 — Rebuilt a supervisor dashboard's client side on WebSockets, taking recurring API calls to 0 (2 remain at initial load). Built NestJS REST APIs behind AI-powered RAG workflows.
- **Freelance** — Sole engineer on an Express.js to NestJS rewrite of a live enrollment API at 100% feature parity, with third-party integrations moved behind a Bull/Redis queue and Redlock on the routes returning duplicate data.
- **Qbatch** · 2021–2023 — Took API response time on a high-traffic application from 200ms to 50ms, mostly indexing after profiling MongoDB queries. Built a production e-commerce backend solo, and consolidated 30+ REST endpoints into a single Redux Toolkit state architecture.

<br />

## 🛠️ Tech Stack

| | |
| :--- | :--- |
| **Languages** | JavaScript, TypeScript, Python, SQL |
| **Frontend** | React.js, Next.js, Redux Toolkit, TanStack Query, Material UI, Tailwind CSS |
| **Backend** | Node.js, Express.js, NestJS, FastAPI, REST APIs, WebSockets, Prisma, BullMQ |
| **Databases** | PostgreSQL, MongoDB, Redis, Snowflake |
| **Testing & Tooling** | Jest, React Testing Library, Playwright, Git, GitHub Actions, Jenkins, Docker |
| **Cloud** | Oracle Cloud, DigitalOcean, Linux |

<br />

📧 [asif.jsdev@gmail.com](mailto:asif.jsdev@gmail.com) — happy to talk about full-stack development, system design, or anything in the projects above.
