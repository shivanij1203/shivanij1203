## Shivani Jagannatham

Software engineer working across AI/ML, data analytics, and backend systems.

Currently AI/ML Engineering and Data Analytics Intern at InnovateK12 and a Research Assistant in USF's Behavioral AI Lab, finishing an MS in Artificial Intelligence and Business Analytics (Dec 2026). Previously Engineer I, Software Development at Verizon, where I shipped Java and Spring Boot services for two years.

I like problems where the bug is in the behavior rather than the stack trace: a streaming parser that corrupts output two tokens later, a connector that reports success after indexing nothing, a model that answers differently when it thinks no one is checking.

### Open source

I contribute fixes to production AI infrastructure.

**[onyx-dot-app/onyx](https://github.com/onyx-dot-app/onyx)** (32k+ stars, open source AI platform)
- Diagnosed why Mistral models broke on every tool call: Onyx appends a user-role reminder after each tool response, which `mistral_common` rejects with a 400 before inference. The investigation was adopted by the maintainers and shipped in [#13539](https://github.com/onyx-dot-app/onyx/pull/13539), credited to my [#12995](https://github.com/onyx-dot-app/onyx/pull/12995).
- [#14721](https://github.com/onyx-dot-app/onyx/pull/14721) (open): the Teams connector caught Microsoft Graph errors without ever logging them, so operators could not tell a 401 from a 403 from a 404. Message retrieval also ran outside its try block, so one failed page ended indexing for an entire team.

**[vitalik/django-ninja](https://github.com/vitalik/django-ninja)** (9k+ stars)
- [#1746](https://github.com/vitalik/django-ninja/pull/1746) (open): `create_schema` crashed on models with a `ForeignObject` reverse relation. The reverse-relation filter matched two subclasses but not their shared base.
- [#1747](https://github.com/vitalik/django-ninja/pull/1747) (open): `ModelSchema` skipped `alias_generator` on foreign key `_id` fields, so those stayed snake_case while every other field was transformed.

### Selected work

**AI and ML**
- [loyalty-audit](https://github.com/shivanij1203/loyalty-audit): black-box detection of hidden loyalties in language models, with no access to weights or activations. Built for Apart Research's Secret Loyalties sprint. The result is a coverage curve showing where behavioral detection catches a hidden loyalty and where it fails structurally.
- [NeoGuard](https://github.com/shivanij1203/NeoGuard): real-time neonatal pain detection. MediaPipe facial landmarks and cry audio analysis, scored with XGBoost and streamed to a nurse dashboard over WebSockets.
- [WageShield](https://github.com/shivanij1203/WageShield): pay stub analyzer that detects wage theft using OCR and retrieval augmented generation.
- [RAISE](https://github.com/shivanij1203/RAISE--Responsible-AI-Standards-and-Ethics): a system of record for AI use in higher education.

**Data**
- [BayAlert](https://github.com/shivanij1203/BayAlert): Tampa Bay water quality monitoring with anomaly detection, two hour forecasting, and upstream to downstream cascade alerts.
- [FiberPulse](https://github.com/shivanij1203/FiberPulse): fiber subscriber analytics with SQL, Python clustering, and Power BI.

**Backend**
- [SpendSmart](https://github.com/shivanij1203/SpendSmart): personal finance tracker with expense categorization and spending analytics.
- [Surplus-Med](https://github.com/shivanij1203/Surplus-Med): medical supply donation platform with automated eligibility checks, multi-tier approval workflows, and audit logging.

### Tools

Python, Java, TypeScript, SQL. Django, FastAPI, Spring Boot, React, Next.js. PostgreSQL, MongoDB, Redshift, dbt. AWS (Bedrock, Lambda, API Gateway, S3), Docker, Git. PyTorch, scikit-learn, XGBoost, OpenCV, MediaPipe.

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/shivani-jagannatham/) · shivanijagannatham@gmail.com
