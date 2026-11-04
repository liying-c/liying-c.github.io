**Software Engineer — Backend · Databases · System Integration**

Backend and data-integration engineer working across SQL, Python, Java/Spring Boot and TypeScript. Own data-migration workflows and translate evolving business requirements into explicit lifecycle rules, API contracts and testable implementations.

**Based in Taipei, Taiwan** · `cliying94 [at] gmail [dot] com` · [GitHub](https://github.com/liying-c) · [LinkedIn](https://www.linkedin.com/in/chen-li-ying) · 中文 · English · Italiano · Deutsch (beg.)

<p class="cv-download-row">
  <a class="cv-download" href="{{ '/Li-Ying_Chen_CV.pdf' | relative_url }}" download="Li-Ying_Chen_CV.pdf" type="application/pdf">Download CV · 1-page PDF</a>
  <small>Updated <time datetime="2026-11-04">4 November 2026</time></small>
</p>

## Selected Highlights

- **Healthcare data migration:** Own Dentall's clinic migration system, reverse-engineering undocumented data models and business semantics across **5 competing HIS products**; the tooling supported onboarding for **20% of new clinic customers in 2025**.
- **Backend design & integration:** Design and implement multi-stage billing workflows and backend APIs for third-party self-service devices, defining lifecycle and settlement boundaries (**in progress**).
- **Cross-language delivery & review:** Work across **Java/Spring Boot, Python and TypeScript** services, translating requirements into data contracts, reviewable changes and verification steps; **150+ merged PRs** and **120+ code reviews** across 8 repositories.
- **Mentoring & delivery:** Mentored **4 classmates** through their first end-to-end delivery of an LLM-backed Android scam detector and Cloudflare Workers gateway, from initial scaffold to v2.1.3 in a **3-week sprint** ([App](https://github.com/SEDIAApp2025/AntifraudApp) · [Gateway](https://github.com/SEDIAApp2025/antifraud-gateway)).

## Experience

### Software Engineer · Dentall Co., Ltd.
*June 2022 – Present · Taipei*

> Dentall builds **dentallHiS**, a cloud-based dental clinic management system with deep National Health Insurance (NHI) integration. My work spans the **Java/Spring Boot core HIS**, **Python migration systems**, and **TypeScript/Node.js integration services**.

#### Clinic Migration System · Project Owner *(2022 – present)*

*Python · SQL · Data Migration · System Architecture*

- Reverse-engineered undocumented schemas, business rules, and workflows across **five competing HIS products** using controlled experiments, database diffs, and Taiwan NHI specifications.
- Built end-to-end migration workflows for clinical records and NHI claims, with pre-flight validation, unattended execution, and resumable checkpoints.
- Built SQL-based migration transformations, including SQL Server XML parsing, relational staging and clinical/claims data mapping.
- Validated migration outcomes through successful NHI claim submissions and XML-level reconciliation of clinical procedures and reimbursement points. The tooling supported onboarding for **20% of new clinic customers in 2025**.
- Delivered a PM-editable spreadsheet/CSV workflow for customer-specific questionnaire conversion, replacing hard-coded mappings with validated inputs, legacy-default fallback and per-run configuration snapshots.
- Plan a component-wise migration-system rebuild around explicit state ownership and retry safety; assess cross-month identifier dependencies before changing the write path (**design stage**).
- Built reusable test environments for product and design teams to explore legacy workflows and validate migration behavior.

#### Billing Workflows & Third-Party Device APIs *(2026 – present; implementation in progress)*

- Proposed the integration architecture and designed over half of the vendor-facing API specification; define access through capability scopes rather than fixed device categories.
- Design and implement core billing workflows, defining when prior-stage amounts become fixed and how subsequent changes produce settlement deltas.
- Define patient-level transaction ownership and locking boundaries that protect the selected billing-record set while allowing amount updates to produce subsequent settlement deltas.
- Resolve business-rule edge cases with product design and frontend engineers; split cross-repository work into reviewable changes and coordinate technical reviews of transaction and cache behaviour.
- Implement the backend in **Java/Spring Boot** and vendor-facing APIs in **TypeScript/Fastify with Firebase**; third-party devices initiate requests and report transaction completion.

#### Java Spring Boot HIS · NHI *(2024 – present)*

- Feature work on NHI billing and drug modules, plus structural cleanup: consolidated the patient-search APIs into a single criteria endpoint, and moved drug reference data out of the HIS into the NHI reference-data service.
- Operability: request-ID tracing in GCP logs, CI test-matrix fix for OOM, and a usage audit that flagged **115 unused endpoints** for deprecation.

#### NHI reference-data service · owner *(2024 – present)*

- Maintain Drugs and Holiday APIs shared by the HIS and card-reader client, with automated reference-data refresh; primary reviewer for the service.

#### Engineering practice

- Direct **AI-assisted development** through scoped tasks, code review and test verification; check generated results against actual input data and output artefacts, not completion summaries.
- Use acceptance criteria, regression checks and CI evidence to review changes; separate release-blocking issues from out-of-scope follow-up work.
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
| **Engineering** | Lifecycle modelling · Transaction boundaries · API / data contracts · Migration validation · Regression testing · Cross-system integration |
| **SQL & Data Processing** | Multi-stage transformations · XML-to-relational mapping · Window functions · Data reconciliation |
| **Backend & Data** | FastAPI · Fastify · Spring Boot · Express · OpenAPI · ETL / migration systems · PostgreSQL · MySQL · SQL Server · SQLite · FoxPro / DBF · BigQuery · Firestore |
| **Cloud & Tooling** | GCP · Firebase · Cloudflare Workers · Azure DevOps · Docker · GitHub Actions · Playwright · Cucumber BDD · Jest / Vitest / Pytest · ISO 27001 / 27701 |
| **Healthcare Domain** | HIS · Taiwan NHI workflows · clinical / claims data migration · structured clinical data · HL7 / FHIR (coursework exposure) |

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
- **Sciwork** &nbsp; *(2023 – present)* — Community volunteer and open-source contributor.

## Languages

**中文** (Native) &nbsp;·&nbsp; **English** (Advanced — daily at Kantar Group) &nbsp;·&nbsp; **Italiano** (Upper-intermediate — Perugia 2017) &nbsp;·&nbsp; **Deutsch** (Beginner)

---

*Last updated: November 2026 · [Source](https://github.com/liying-c/liying-c.github.io)*
