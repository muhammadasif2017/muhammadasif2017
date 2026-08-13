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

I build web applications end to end, from the interface down to the data layer. Four years of it so far, mostly TypeScript — enterprise platforms, an e-commerce backend, and a customer enrollment system handling live sign-ups.

Open to full-stack and backend engineering roles.

<br />

## 🚀 What I Do

- **Frontend engineering** — React, Next.js and TypeScript, including reusable component libraries that several backend services feed into.
- **Backend development** — REST APIs, business logic and integrations in Node.js and NestJS.
- **Real-time features** — WebSocket and event-driven work, mostly replacing polling that was costing more than it was worth.
- **Performance work** — Profiling slow paths and fixing them. Usually database queries, sometimes the fetching layer above them.
- **Modernizing existing code** — Migrations and refactors on live systems, without changing behaviour for the people using them.

<br />

## 💼 Engineering Experience

**Afiniti** — Rebuilt the client side of a supervisor dashboard on WebSockets. It had been polling two agent-data endpoints on a timer, which kept re-fetching records that hadn't changed and left the view stale between polls. Recurring API calls went to 0, with 2 left at initial load. Also built NestJS REST APIs behind AI-powered RAG workflows, wiring external LLM services to internal knowledge sources.

**Freelance, California LifeLine enrollment platform** — Sole engineer on an Express.js to NestJS rewrite of a live REST API at 100% feature parity. Put the third-party integrations behind a Bull/Redis queue with a dashboard for job state and failures, and added Redlock on the routes where concurrent requests were returning duplicate data.

**Qbatch** — Got API response time on a high-traffic application down from 200ms to 50ms. Mostly indexing after profiling the MongoDB queries, plus a few rewrites. Also built the entire backend for a production e-commerce app solo, and consolidated 30+ REST endpoints into a single Redux Toolkit state architecture.

<br />

## 📂 Projects

### 🗂️ &nbsp;[Job Tracker](https://github.com/muhammadasif2017/job-tracker)

An application for tracking job applications through each stage of a search. I built it because I needed one, and I use it daily.

- JWT access/refresh auth plus Google and GitHub OAuth2, using a server-side code exchange so tokens never appear in redirect URLs
- Company enrichment pulled from external services through an async BullMQ pipeline with retries and failure handling
- Resume storage behind a swappable driver interface — local disk in dev, Oracle Object Storage in prod
- Runs in production on Oracle Cloud. Pull-based CI/CD, Jest and Playwright e2e tests against a live database

<sub>**NestJS** · PostgreSQL · Prisma · Next.js 16 · React 19 · TypeScript · BullMQ · Docker</sub>

### 🔐 &nbsp;[Nest Nexus](https://github.com/muhammadasif2017/nest-nexus)

A NestJS backend that implements 6 different ways of signing in, each one properly. Most auth examples stop at a JWT and a login form, so I wanted a reference that went further.

- JWT with refresh-token rotation, OAuth2, TOTP 2FA, magic links, WebAuthn passkeys, API keys
- Token-family reuse detection on rotation, with atomic revoke-then-issue sequencing to block replay
- Event-driven cache invalidation over EventEmitter2 and Redis Pub/Sub
- 17+ architecture decision records in the repo, if you want the reasoning behind any of it

<sub>**NestJS** · TypeScript · PostgreSQL · Prisma · Redis · BullMQ · Docker · Caddy</sub>

<br />

## 🛠️ Tech Stack

| | |
| :--- | :--- |
| **Languages** | JavaScript, TypeScript, HTML, CSS, SQL |
| **Frontend** | React.js, Next.js, Redux Toolkit, TanStack Query, Material UI, Tailwind CSS |
| **Backend** | Node.js, Express.js, NestJS, REST APIs, WebSockets, Prisma, BullMQ |
| **Databases** | PostgreSQL, MongoDB, Redis, Snowflake |
| **Testing & Tooling** | Jest, React Testing Library, Playwright, Git, GitHub Actions, Jenkins, Docker |
| **Cloud** | Oracle Cloud, DigitalOcean, Linux |

<br />

## 📌 Currently Focused On

- Backend architecture with Node.js and NestJS
- API design, and the parts of system design I've had to learn by getting them wrong first
- AI-powered applications — RAG workflows and LLM integrations, which I first worked on at Afiniti and have kept building on since

<br />

## 🤝 Let's Connect

Happy to talk about full-stack development, system design, or anything in the projects above.

📧 **Email** — [asif.jsdev@gmail.com](mailto:asif.jsdev@gmail.com)
💼 **Open to** — full-stack and backend engineering roles, remote or Lahore
⭐ If one of the repos is useful to you, a star is always welcome
