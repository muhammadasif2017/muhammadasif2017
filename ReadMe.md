<h1 align="center">Muhammad Asif</h1>

<p align="center">
  Full-Stack Engineer &nbsp;·&nbsp; Node.js / NestJS / React / Next.js &nbsp;·&nbsp; Lahore, Pakistan
</p>

<p align="center">
  <a href="https://linkedin.com/in/asif-jsdev">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:asif.jsdev@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://github.com/muhammadasif2017">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Open%20to%20work-Full--Stack%20%2F%20Backend-2ea44f?style=flat-square" alt="Open to work" />
  <img src="https://img.shields.io/badge/Experience-4%2B%20years-blue?style=flat-square" alt="4+ years" />
  <img src="https://img.shields.io/badge/Remote%20or%20Lahore-informational?style=flat-square" alt="Location" />
</p>

---

### About

Four years building web applications, most of it in JavaScript and TypeScript. I started out frontend-heavy with React and moved toward the backend over time — the last engagement I took was server-side only. Two product companies in Lahore before that.

I'm currently looking for a full-stack or backend role, remote or onsite in Lahore. Email is the fastest way to reach me: **asif.jsdev@gmail.com**

---

### Work worth mentioning

**Afiniti** — Rebuilt the client side of a supervisor dashboard on WebSockets. It had been polling two agent-data endpoints on a timer, which kept re-fetching records that hadn't changed and left the view stale between polls. Recurring API calls went to 0, with 2 left at initial load. React, Next.js, TypeScript, Redux.

**Freelance (California LifeLine enrollment platform)** — Sole engineer on an Express.js to NestJS rewrite of a live REST API at 100% feature parity. Put the third-party integrations behind a Bull/Redis queue with a dashboard for job state and failures, and added Redlock on the routes where concurrent requests were returning duplicate data.

**Qbatch** — Got API response time on a high-traffic application down from 200ms to 50ms. Mostly indexing after profiling the MongoDB queries, plus a few rewrites. Also built the entire backend for a production e-commerce app solo.

---

### Tech

**Languages**

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-DD2C00?style=flat-square&logo=redis&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Redux Toolkit](https://img.shields.io/badge/Redux%20Toolkit-764ABC?style=flat-square&logo=redux&logoColor=white)
![TanStack Query](https://img.shields.io/badge/TanStack%20Query-FF4154?style=flat-square&logo=reactquery&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Material UI](https://img.shields.io/badge/Material%20UI-007FFF?style=flat-square&logo=mui&logoColor=white)

**Data**

![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)

**Infra & testing**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Oracle Cloud](https://img.shields.io/badge/Oracle%20Cloud-F80000?style=flat-square&logo=oracle&logoColor=white)
![DigitalOcean](https://img.shields.io/badge/DigitalOcean-0080FF?style=flat-square&logo=digitalocean&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)

---

### Projects

<table>
<tr>
<td width="50%" valign="top">

#### [Job Tracker](https://github.com/muhammadasif2017/job-tracker)

Full-stack application for tracking job applications, running in production on Oracle Cloud.

- JWT access/refresh auth plus Google and GitHub OAuth2, using a server-side code exchange so tokens never appear in redirect URLs
- Company-enrichment services pulled through an async BullMQ pipeline with retries and failure handling
- Drag-and-drop kanban board with optimistic updates and rollback
- Resume storage behind a swappable driver interface — local disk in dev, Oracle Object Storage in prod
- Pull-based CI/CD, Jest and Playwright e2e tests against a live database

`NestJS` `PostgreSQL` `Prisma` `Next.js 16` `React 19` `TypeScript` `BullMQ` `Docker`

</td>
<td width="50%" valign="top">

#### [Nest Nexus](https://github.com/muhammadasif2017/nest-nexus)

A NestJS backend built around authentication, written to show the patterns properly rather than the minimum that works.

- 6 authentication methods: JWT with refresh-token rotation, OAuth2, TOTP 2FA, magic links, WebAuthn passkeys, API keys
- Token-family reuse detection on rotation, with atomic revoke-then-issue sequencing to block replay
- Event-driven cache invalidation over EventEmitter2 and Redis Pub/Sub
- BullMQ pipeline with dead-letter handling, health checks, structured logging
- 17+ architecture decision records in the repo

`NestJS` `TypeScript` `PostgreSQL` `Prisma` `Redis` `BullMQ` `Docker` `Caddy`

</td>
</tr>
</table>

---

### GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=muhammadasif2017&show_icons=true&hide_border=true&bg_color=00000000&title_color=3178C6&text_color=808080&icon_color=3178C6" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=muhammadasif2017&layout=compact&hide_border=true&bg_color=00000000&title_color=3178C6&text_color=808080&langs_count=8" alt="Top languages" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=muhammadasif2017&hide_border=true&bg_color=00000000&color=808080&line=3178C6&point=3178C6&area=true" alt="Contribution graph" />
</p>

---

### Elsewhere

- **Email** — [asif.jsdev@gmail.com](mailto:asif.jsdev@gmail.com)
- **LinkedIn** — [asif-jsdev](https://linkedin.com/in/asif-jsdev)
- **Education** — BSc. Computer Science, University of Engineering & Technology, Lahore (2021)
