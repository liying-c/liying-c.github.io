> **Software engineer (5+ yrs)** at a healthcare SaaS that's adopted **AI-mandated development** — shipping production code in a daily AI-paired workflow. Incoming M.S. — Digital Twin research (Sep 2026 · Fu Jen Catholic University). Based in Taipei.
>
> `cliying94 [at] gmail [dot] com` · [GitHub](https://github.com/liying-c) · [LinkedIn](https://www.linkedin.com/in/chen-li-ying) · 中文 / English / Italiano / Deutsch (beg.)

## Selected Highlights

- **Primary engineer** on Dentall's partner-facing API platform — designed a **least-privilege API-key permission model** (resource × action scopes) replacing a prior all-or-nothing token scheme.
- Co-built a **heterogeneous data-migration toolchain** across **FoxPro / dBase, SQL Server, MySQL, PostgreSQL and SQLite** — moved **~20% of targeted competing-system clinics** onto Dentall in year one.
- Owns key **NHI-integration modules** inside dentallHiS — monthly-declarations API, partial-burden-discount reporting, and accounting aligned with Taiwan's evolving claim rules.
- **Daily AI-assisted engineering practice** — pair with Claude AI on code design, refactor planning, review and ad-hoc tooling across work and side projects.
- Mentored **4 classmates** through their first end-to-end ship — an LLM-backed Android scam detector + Cloudflare-Workers edge gateway, **3-week sprint** from scaffold to v2.1.3.

## Skills

| Area | Stack |
|------|-------|
| **Languages** | Java · Python · SQL · TypeScript · C# · JavaScript · Shell |
| **AI Workflow** | Claude AI (daily engineering collaborator) · LLM integration (Llama 3) · prompt design · agent / tool use patterns |
| **Backend** | Spring Boot · FastAPI · Express · Flask · Gradio |
| **Cloud / Edge** | Cloudflare Workers · GCP (BigQuery, Pub/Sub, Cloud Storage) · Azure DevOps · Docker · Linux |
| **Data & Databases** | ETL pipeline design · schema migration · PostgreSQL · MySQL · SQL Server · BigQuery · SQLite · FoxPro / DBF · Firebase / Firestore |
| **Quality & Tooling** | Playwright (E2E) · Cucumber BDD · Jest · Vitest · Pytest · OpenAPI / Swagger · GitHub Actions · ISO 27001 / 27701 |

## Experience

### Software Engineer · Dentall Co., Ltd.
*June 2022 – Present · Taipei*

> Dentall builds **dentallHiS**, a cloud-based dental clinic management system with deep National Health Insurance (NHI) integration.

- **Designed and shipped the partner-facing API authorization layer** (V2 API-key auth + OAuth-style scope mechanism + CLI provisioning) — written up below under *Featured Projects · Dentall External API*.
- **Owns NHI-integration modules** in dentallHiS — monthly-declarations API with upload-serial isolation, partial-burden-discount reporting, and accounting integration against Taiwan's evolving NHI claim rules.
- **Co-built a heterogeneous data-migration toolchain** spanning **FoxPro / dBase, SQL Server, MySQL, PostgreSQL and SQLite**, orchestrated end-to-end via docker-compose (init → DB migration → XML migration → patch → export); moved **~20% of targeted competing-system clinics** onto Dentall in year one.
- **Built a FastAPI + Gradio analytics interface** for an internal healthcare-AI initiative — chosen so non-engineers on the team could prototype against clinical datasets directly.
- **Drove BDD adoption** with Cucumber feature files written in **domain-Chinese**, keeping PM / QA / engineering on shared vocabulary; introduced Playwright (TypeScript) E2E to the release workflow.
- Participating in an **ongoing team-wide refactor toward DDD-style module boundaries** (codebase is not yet DDD); contributed to **ISO 27001 / ISO 27701** compliance reviews.

### Database Programmer · Kantar Taiwan *(Kantar Group)*
*April 2021 – May 2022 · Taipei*

- Owned database administration — maintenance, schema changes and data updates — for internal BI systems.
- Built non-standardized **ETL pipelines** in C# and Python to serve research-team requests.
- Authored **English-language technical documentation** to support cross-team collaboration across Kantar offices.
- Introduced **Azure DevOps** for source control and release management.
- Stood up a **GCP** environment to evaluate the feasibility of image-recognition workflows.

## Featured Projects

### Dentall External API — Authorization System Design
*Designer & primary engineer · Mar 2026 – present · Node.js / TypeScript / Fastify 5 / Firestore*

Two-phase design and shipped Dentall's partner-facing API authorization layer — Firestore-backed V2 API-key authentication, an OAuth-style scope mechanism, and the CLI tooling that provisions and manages keys end-to-end.

- **OAuth-style scope mechanism** (`resource:action`) — per-route scope-check hook with structured 403.
  - Explored a Phase 2 refactor moving the rule store from a source-code lookup table → a per-key Firestore field (with migration + verify scripts and a strict deploy order to avoid 403 storms).
  - After re-evaluating cost vs current need, **shipped the simpler Phase 1 (lookup table)** and documented Phase 2 as a future-option for when per-key override actually lands as a requirement.
  - **Zero vender-facing breaking change.**
- **CLI provisioning tooling** — direct Firestore via Firebase Auth Google SSO (key creation never traverses HTTP). Commands cover create / list / suspend / activate / revoke + admin account bootstrap; vender vs admin RBAC with per-vender ownership isolation.

*270+ Vitest unit + integration tests covering auth and scope surfaces.*

### SEDIA Antifraud — Android scam detector + Edge API gateway
*Lead developer & mentor · 4-classmate student team · Dec 2025 – Jan 2026 (~3-week sprint)* · [App](https://github.com/SEDIAApp2025/AntifraudApp) · [Gateway](https://github.com/SEDIAApp2025/antifraud-gateway)

Hand-coded the TypeScript gateway and AI-paired the Kotlin Android shell from my architecture spec; then onboarded four classmates and mentored them from Git fundamentals through PR-based review across **10+ feature PRs** to v2.1.3. Integrates Google Safe Browsing, a scam phone-number dataset, and an LLM (Llama 3) text-analysis path behind a Cloudflare Workers edge gateway.

- **Cloudflare Workers gateway (TypeScript)** — `x-api-key` auth, auto-generated OpenAPI / Swagger UI, semver-tagged GitHub Actions release flow, LLM response parser with JSON-truncation repair.
- **Specified API-key hardening** on the Android side — upstream key pushed into a native NDK / C++ / CMake layer so it never ships in the APK.

## Education & Research

**Fu Jen Catholic University** &nbsp; Incoming Master of Engineering — Department of Computer Science and Information Engineering &nbsp; *(Sep 2026 –)*
- Already joined the lab; research topic confirmed: **Digital Twin for ESG / Life Cycle Assessment**.
- *Preliminary research work:* [`simapro-preprocess`](https://github.com/liying-c/simapro-preprocess) — Python CLI for cleaning SimaPro CSV exports (ISO 14040 LCA), used to bootstrap the lab's LCI conventions.

**Fu Jen Catholic University** &nbsp; Bachelor of Engineering — Bachelor's Program in Software Engineering and Digital Innovation Application &nbsp; *(2024 – present)*

**Fu Jen Catholic University** &nbsp; B.A., Italian Language & Culture / Physical Education &nbsp; *(2014 – 2019)* — incl. summer at **Università per Stranieri di Perugia** *(2017)*

## Community

- **Taipei.py** &nbsp; Co-organizer *(current)* — help run meetups for the Taipei Python community.
- **PyCon Taiwan** &nbsp; *(2021 – present)* — Volunteer on Registration, Development and Program teams; small contribution to `pycontw/PyCon-ETL`.
- **Sciwork** &nbsp; *(2023 – present)* — Sprint co-organizer and event volunteer.

## Languages

**中文** (Native) &nbsp;·&nbsp; **English** (Advanced — daily at Kantar Group) &nbsp;·&nbsp; **Italiano** (Upper-intermediate — Perugia 2017) &nbsp;·&nbsp; **Deutsch** (Beginner)

---

*Last updated: May 2026 · [Source](https://github.com/liying-c/liying-c.github.io)*
