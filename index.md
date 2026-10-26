> **Software Engineer | Backend · Databases · System Integration** — building and maintaining production systems across Java/Spring Boot, Python, and TypeScript. Focused on database integration, data migration, API design, and translating complex business workflows into maintainable software. Based in Taipei.
>
> `cliying94 [at] gmail [dot] com` · [GitHub](https://github.com/liying-c) · [LinkedIn](https://www.linkedin.com/in/chen-li-ying) · 中文 / English / Italiano / Deutsch (beg.)

## Selected Highlights

- **Healthcare data migration:** Own Dentall's clinic migration system, reverse-engineering undocumented data models and business semantics across **5 competing HIS products**; the system supported transitions representing **20% of clinics in one year**.
- **Domain modeling & system integration:** Design lifecycle and transaction boundaries for a self-service kiosk integration, reducing dependencies between evolving billing stages and external device workflows (implementation in progress).
- **Production engineering & reviews:** Work across a **Java/Spring Boot core system**, **Python migration and data-processing workflows**, and **TypeScript external APIs**; contributed **150+ merged PRs** and **120+ code reviews** across 8 repositories.
- **Mentoring & delivery:** Mentored **4 classmates** through their first end-to-end delivery of an LLM-backed Android scam detector and Cloudflare Workers gateway, from initial scaffold to v2.1.3 in a **3-week sprint** ([App](https://github.com/SEDIAApp2025/AntifraudApp) · [Gateway](https://github.com/SEDIAApp2025/antifraud-gateway)).

## Experience

### Software Engineer · Dentall Co., Ltd.
*June 2022 – Present · Taipei*

> Dentall builds **dentallHiS**, a cloud-based dental clinic management system with deep National Health Insurance (NHI) integration. My work spans the **Java/Spring Boot core HIS**, **Python migration systems**, and **TypeScript/Node.js integration services**.

#### Clinic migration system · owner *(2022 – present)*

- Reverse-engineer undocumented data models, business semantics, and workflows across **5 competing HIS products** through controlled experiments and database diffs to derive migration mappings.
- Built the end-to-end migration flow for clinical records and NHI claim history, with pre-flight checks, unattended execution, and resumable checkpoints, plus reusable test environments for PM and design to study legacy workflows and validate migrations.
- The system became the entry point for customers switching to Dentall; **20% of clinics transitioned and became clients in one year**.
- Reviewing the architecture of a legacy Python migration system, identifying Java-style object modeling, differences in class and instance lifecycle assumptions, and implicit state dependencies. Working with the engineering lead to define clearer transformation, state-ownership, and execution boundaries.

#### External API · self-service clinic systems *(2026 – present)*

- Define API and system boundaries between the HIS and configurable self-service check-in / cash-deposit kiosks under incomplete and evolving vendor specifications.
- Model multi-stage billing lifecycles and delta-based settlement adjustments; propose freezing prior-stage instances when a successor is created to limit cross-stage mutable-state dependencies.
- Design person-scoped settlement boundaries around a Freeze API and device-issued transaction IDs, with explicit rules for eligible documents and completed transactions. Concurrency, recovery, and device integration behavior remain under implementation and verification.
- Collaborate with product design, frontend engineering, and senior reviewers to refine incomplete requirements and challenge cross-system synchronization assumptions.
- Proposed the integration architecture, scoped device API-key model, and over half of the API surface; evolved a vendor's legacy SOAP specification into a REST contract through repeated specification and architecture reviews.
- Develop external APIs with **Fastify / TypeScript on Firebase**, including CLI-based device-key provisioning.

#### Java Spring Boot HIS · NHI *(2024 – present)*

- Feature work on NHI billing and drug modules, plus structural cleanup: consolidated the patient-search APIs into a single criteria endpoint, and moved drug reference data out of the HIS into the NHI reference-data service.
- Operability: request-ID tracing in GCP logs, CI test-matrix fix for OOM, and a usage audit that flagged **115 unused endpoints** for deprecation.

#### NHI reference-data service · owner *(2024 – present)*

- Maintain Drugs and Holiday APIs shared by the HIS and card-reader client, with automated reference-data refresh; primary reviewer for the service.

#### Engineering practice

- Use **AI-assisted development** to accelerate implementation, exploration, and iteration while retaining responsibility for system design, code review, tests, and validation.
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

## Education

**Fu Jen Catholic University** &nbsp; Undergraduate Coursework — Bachelor's Program in Software Engineering and Digital Innovation Application &nbsp; *(2024 – 2026; degree not completed)*

- **GPA: 4.0 / 4.0**
- **Core coursework:** Data Structures, Operating Systems, Computer Networks, Object-Oriented Programming, Discrete Mathematics, Data Science Programming, Calculus, and Linear Algebra.
- **Graduate-level coursework:** Software Design Patterns and Information Visualization; Management Information Systems *(in progress)*.
- **Health Informatics:** HL7, FHIR, structured clinical data, and healthcare information-system architecture.

**Fu Jen Catholic University** &nbsp; B.A., Italian Language & Culture &nbsp; *(2014 – 2019)* — incl. summer at **Università per Stranieri di Perugia** *(2017)*

- **Earlier interdisciplinary coursework in athletic training, sports medicine, and exercise science:** Anatomy, Kinesiology, Exercise Physiology, Sports Injuries and First Aid, Sports Nutrition, and Exercise and Health Promotion.
- **Music:** university-level coursework in percussion, ensemble performance, jazz, and musicianship, building on 10 years of formal music training.

## Community

- **Taipei.py** &nbsp; Co-organizer *(current)* — help run meetups for the Taipei Python community.
- **PyCon Taiwan** &nbsp; *(2021 – present)* — Volunteer across Registration, Development, and Program teams; contributed to `pycontw/PyCon-ETL`.
  - **2026 Program Team / Keynote Host:** Supported the talk lifecycle, including proposal reviews, speaker communications, review decisions and responses, and session coordination; hosted an English-language keynote session.
- **Sciwork** &nbsp; *(2023 – present)* — Sprint co-organizer and event volunteer.

## Languages

**中文** (Native) &nbsp;·&nbsp; **English** (Advanced — daily at Kantar Group) &nbsp;·&nbsp; **Italiano** (Upper-intermediate — Perugia 2017) &nbsp;·&nbsp; **Deutsch** (Beginner)

---

*Last updated: October 2026 · [Source](https://github.com/liying-c/liying-c.github.io)*
