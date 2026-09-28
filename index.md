> **Software engineer focused on backend and data-intensive systems** — working across migration/ETL, system integration, APIs, and domain-heavy production software. Most of my recent domain experience is in healthcare. Incoming M.S. — Digital Twin research (Sep 2026 · Fu Jen Catholic University). Based in Taipei.
>
> `cliying94 [at] gmail [dot] com` · [GitHub](https://github.com/liying-c) · [LinkedIn](https://www.linkedin.com/in/chen-li-ying) · 中文 / English / Italiano / Deutsch (beg.)

## Selected Highlights

- **Own the clinic migration system** at Dentall — reverse-engineer undocumented data models and semantics across **5 competing HIS products**; the system helped **20% of clinics transition and become clients in one year**.
- Define **system and API boundaries** for self-service clinic kiosk integrations, including workflows where HIS-side and kiosk-side payment state may exist independently or together.
- Mentored **4 classmates** through their first end-to-end ship — an LLM-backed Android scam detector + Cloudflare Workers gateway, **3-week sprint** from scaffold to v2.1.3 ([App](https://github.com/SEDIAApp2025/AntifraudApp) · [Gateway](https://github.com/SEDIAApp2025/antifraud-gateway)).

## Experience

### Software Engineer · Dentall Co., Ltd.
*June 2022 – Present · Taipei*

> Dentall builds **dentallHiS**, a cloud-based dental clinic management system with deep National Health Insurance (NHI) integration.

#### Clinic migration system · owner *(2022 – present)*

- Reverse-engineer undocumented data models, business semantics, and workflows across **5 competing HIS products** through controlled experiments and database diffs to derive migration mappings.
- Built the end-to-end migration flow for clinical records and NHI claim history, with pre-flight checks, unattended execution, and resumable checkpoints, plus reusable test environments for PM and design to study legacy workflows and validate migrations.
- The system became the entry point for customers switching to Dentall; **20% of clinics transitioned and became clients in one year**.
- Currently redesigning transformations so product can define migration rules independently of execution logic, while the system provides **validation, idempotency, resumability, and auditability**; refactoring the legacy Java-shaped Python codebase toward idiomatic state, transformation, and execution boundaries.

#### External API · self-service clinic systems *(2026 – present)*

- Define API and system boundaries between the HIS and configurable self-service check-in / cash-deposit kiosks under incomplete and evolving vendor specifications.
- Model workflows spanning **HIS-side, kiosk-side, and combined payment states**, where the two systems may own partially independent transaction state.
- Proposed the integration architecture, scoped device API-key model, and over half of the API surface; evolved a vendor's legacy SOAP specification into a REST contract through repeated specification and architecture reviews.
- Implemented with **Fastify / TypeScript on Firebase**, with CLI-based provisioning.

#### Java Spring Boot HIS · NHI *(2024 – present)*

- Feature work on NHI billing and drug modules, plus structural cleanup: consolidated the patient-search APIs into a single criteria endpoint, and moved drug reference data out of the HIS into the NHI reference-data service.
- Operability: request-ID tracing in GCP logs, CI test-matrix fix for OOM, and a usage audit that flagged **115 unused endpoints** for deprecation.

#### NHI reference-data service · owner *(2024 – present)*

- Maintain Drugs and Holiday APIs shared by the HIS and card-reader client, with automated reference-data refresh; primary reviewer for the service.

#### Engineering practice

- **150+ merged PRs** and **120+ code reviews** across 8 repositories.
- Participate in ISMS / ISO 27001 and 27701 business-continuity drills and internal technical knowledge sharing.
- Earlier projects include a **FastAPI + Gradio** analysis system for internal AI work and a **Playwright** end-to-end testing prototype.

### Database Programmer / Maintainer · Kantar Taiwan *(Kantar Group)*
*April 2021 – May 2022 · Taipei*

- Independently developed customer-specific **ETL features** for an internal BI platform using SQL Server and C#, including workflows handling personal data under GDPR requirements, working with cross-regional teams across cultures and time zones.
- Introduced engineering practices and technologies new to the team, including GCP and Azure, Azure DevOps / TFS version-control workflows, MVVM architecture, and TDD concepts.
- Built a **GCP environment from scratch** to evaluate image-recognition feasibility for a client project.

## Skills

| Area | Stack |
|------|-------|
| **Languages** | Python · TypeScript · SQL · Java · C# · JavaScript · Shell |
| **Backend & Data** | FastAPI · Fastify · Spring Boot · Express · OpenAPI · ETL / migration systems · PostgreSQL · MySQL · SQL Server · SQLite · FoxPro / DBF · BigQuery · Firestore |
| **Cloud & Tooling** | GCP · Firebase · Cloudflare Workers · Azure DevOps · Docker · GitHub Actions · Playwright · Cucumber BDD · Jest / Vitest / Pytest · ISO 27001 / 27701 |
| **Healthcare Domain** | HIS · Taiwan NHI workflows · clinical / claims data migration · HL7 · FHIR · structured clinical data |

## Education & Research

**Fu Jen Catholic University** &nbsp; Incoming Master of Engineering — Department of Computer Science and Information Engineering &nbsp; *(Sep 2026 –)*
- Already joined the lab; research topic confirmed: **Digital Twin for ESG / Life Cycle Assessment**.
- *Preliminary research work:* [`simapro-preprocess`](https://github.com/liying-c/simapro-preprocess) — Python CLI for cleaning SimaPro CSV exports (ISO 14040 LCA), used to bootstrap the lab's LCI conventions.

**Fu Jen Catholic University** &nbsp; Undergraduate Studies — Bachelor's Program in Software Engineering and Digital Innovation Application &nbsp; *(2024 – present)*

- **GPA: 4.0 / 4.0**
- **Core coursework:** Data Structures, Operating Systems, Computer Networks, Object-Oriented Programming, Discrete Mathematics, Data Science Programming, Calculus, and Linear Algebra.
- **Graduate-level coursework:** Software Design Patterns and Information Visualization; Management Information Systems *(in progress)*.
- **Health Informatics:** HL7, FHIR, structured clinical data, and healthcare information-system architecture.

**Fu Jen Catholic University** &nbsp; B.A., Italian Language & Culture &nbsp; *(2014 – 2019)* — incl. summer at **Università per Stranieri di Perugia** *(2017)*

- **Earlier interdisciplinary coursework in athletic training, sports medicine, and exercise science:** Anatomy, Kinesiology, Exercise Physiology, Sports Injuries and First Aid, Sports Nutrition, and Exercise and Health Promotion.
- **Music:** university-level coursework in percussion, ensemble performance, jazz, and musicianship, building on 10 years of formal music training.

## Community

- **Taipei.py** &nbsp; Co-organizer *(current)* — help run meetups for the Taipei Python community.
- **PyCon Taiwan** &nbsp; *(2021 – present)* — Volunteer on Registration, Development and Program teams; small contribution to `pycontw/PyCon-ETL`.
- **Sciwork** &nbsp; *(2023 – present)* — Sprint co-organizer and event volunteer.

## Languages

**中文** (Native) &nbsp;·&nbsp; **English** (Advanced — daily at Kantar Group) &nbsp;·&nbsp; **Italiano** (Upper-intermediate — Perugia 2017) &nbsp;·&nbsp; **Deutsch** (Beginner)

---

*Last updated: September 2026 · [Source](https://github.com/liying-c/liying-c.github.io)*
