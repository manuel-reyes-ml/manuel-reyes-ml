# Hi, I'm Manuel 👋

### Analytics Engineer · Data Engineer — AI-ready data platforms

🟢 **Open to Analytics Engineer and Data Engineer roles** — especially teams building **AI-ready data** (semantic layers, embedding pipelines, evaluation-gated AI). **Available now.**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-mr410-0077B5?logo=linkedin)](https://www.linkedin.com/in/mr410/)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?logo=gmail&logoColor=white)](mailto:manuelreyesv410@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-data--portfolio-667eea)](https://github.com/manuel-reyes-ml/data-portfolio)
[![Roadmap](https://img.shields.io/badge/Roadmap-v10.0-28a745)](https://manuel-reyes-ml.github.io/learning_journey/roadmap.html)

I build data pipelines that have to be right — where a wrong number becomes a wrong tax form. My reconciliation pipeline runs in production in an ERISA-regulated retirement-plan operation, and I'm hardening it in public into a dbt-modelled data platform. I bring **15+ years of business operations** (manufacturing, digital marketing), **2 years of ERISA retirement-plan operations** (1099-R reporting, distribution QA) and **5+ years of independent trading** — so I model the business before I model the data.

---

## 🧾 Start here — a pipeline that runs in production

**[1099 Reconciliation Pipeline → DataVault](https://github.com/manuel-reyes-ml/1099_reconciliation_pipeline)** reconciles retirement-plan distributions across two recordkeeping systems, derives the expected 1099-R Box-7 code, and produces correction files for human review.

| Metric | Impact |
|---|---|
| ⚡ Effort | **~95% reduction** in weekly reconciliation effort |
| 📈 Scale | The **full distribution book**, without added headcount |
| 🛡️ Correctness | **Derived-vs-reported Box-7 validation gate** — mismatches quarantined before distribution |
| ✅ Reliability | Reconciliation success rate held against a stated **freshness SLA** |

**Now (DataVault, Stage 2):** reconciliation rules rebuilt as **dbt models with a unit test per rule** (`dbt build` gating every PR, published dbt docs) → Polars ingestion with row-level contracts → Airflow → Docker/ECS → monitoring and a written postmortem. The shipped pandas version stays frozen as the *before*; the measured delta is the headline.

> 🔒 Public repos use **synthetic data only**. Claims are limited to mechanism and relative deltas — no participant, plan, client or employer-identifying data.

---

## 🏆 Portfolio

Ordered by the roles I'm targeting. Status: ✅ live · 🏗️ in build · 📐 designed · 📅 planned

| Project | What it proves | For | Status |
|---|---|---|---|
| **[DataVault / 1099 Data Platform](https://github.com/manuel-reyes-ml/1099_reconciliation_pipeline)** | Live reconciliation ETL → dbt-tested models with a declared grain, data contracts, orchestration and a semantic layer | AE · DE | ✅ S1 live · 🏗️ S2 |
| **[PostCheck](https://github.com/manuel-reyes-ml/postcheck)** | Read-only QA agent for posted distributions: exactly-once ingestion → append-only event log → dbt quality mart. The blocking gate is false-NIGO rate, not accuracy | AE · DE · AI | 📐 |
| **[PolicyPulse](https://github.com/manuel-reyes-ml/policypulse)** | Cited-answer RAG → GraphRAG over plan documents; access control enforced at retrieval; RAGAS/DeepEval gates block merges; FastMCP server | Applied AI | 🏗️ |
| **[Crucible](https://github.com/manuel-reyes-ml/crucible)** | Backtest → paper → live trading platform where a deterministic core owns every order — human sign-off, kill-switch, the LLM sees aggregates only | Applied AI · safety | 🏗️ |
| [AFC](https://github.com/manuel-reyes-ml/attention-flow-catalyst) *(supporting)* | AI-powered predictive trigger analysis for small caps: point-in-time event study + ML meta-labeling, reported as calibrated lift with false-discovery control — never returns | Applied AI · data | 🏗️ |
| [FormSense](https://github.com/manuel-reyes-ml/formsense) *(supporting)* | Multimodal extraction of distribution forms against a frozen Pydantic contract, with schema-adherence gates and low-confidence routing | Applied AI | 📅 |

**Full write-ups** — Production · Cost · Architecture for every project, scope documents and the production standard → **[data-portfolio](https://github.com/manuel-reyes-ml/data-portfolio)**

---

## 🛠️ How I build

- **Evaluation gates block merges.** RAGAS / DeepEval / GEval thresholds are CI conditions, and the metric fits the cost of being wrong — a review agent that cries wolf loses the trust it needs.
- **Business logic lives in tested dbt models.** Declared grain, a test per rule, contracts at the boundaries. Polars owns ingestion; pandas stays only at the Excel-template and plotting edges — recorded as an ADR.
- **Reproducible and enforced.** Python 3.14 pinned once, a committed `uv.lock`, `uv sync --frozen` in CI and Docker. Pinned pre-commit hooks (a strict subset of CI) with `gitleaks` and `nbstripout` make *synthetic data only* mechanical.
- **Observable by construction.** `structlog` renders my logs and my dependencies' through one chain with a PII-redaction processor; typed config (`pydantic-settings`); capped retries (`stamina`).
- **Decisions are written down, and AI assists — it doesn't author.** ADRs with rejected alternatives and a C4 diagram in every repo; branch → PR → review → merge; agents can't commit, so every line is reviewed by me.

---

## 🧰 Stack

| Tier | Tools |
|---|---|
| **Shipped** | Python · pandas · openpyxl · pytest · GitHub Actions · uv · pre-commit · Pydantic · Faker (synthetic data) |
| **Building now** | SQL · dbt Core + DuckDB · Polars · Docker · structlog · Anthropic SDK · RAG · FastMCP · DeepEval · RAGAS |
| **Stage 2** | Snowflake · Airflow · Great Expectations · AWS (S3, ECS) · Terraform · PySpark · Power BI semantic layer |
| **Stage 3** | GraphRAG (Neo4j) · LangGraph · Azure AI Foundry · Vercel AI SDK (TypeScript last mile) |

**Domain:** 1099-R reporting and distribution codes · ERISA retirement-plan operations (403(b), 457, IRA, Roth) · Relius · Matrix · OnBase

---

## 🗺️ Path — 3 stages, evidence-gated

| Stage | Focus | Status |
|---|---|---|
| **1** · Months 1–8 | Production Python, SQL + dbt, eval-first AI — *the build work* | 🟢 Active — exits when DataVault S2 ships |
| **2** · Months 9–20 | **Analytics Engineer** (first door) · **Data Engineer** — AI-ready data | 🎯 Target role |
| **3** · Months 21–32 | Applied AI Engineer → Forward-Deployed Engineer | 🎯 Long term |

What I'm studying and why → **[learning_journey](https://github.com/manuel-reyes-ml/learning_journey)** · every decision and its rationale → **[roadmap](https://manuel-reyes-ml.github.io/learning_journey/roadmap.html)**

---

## 🎓 Education & credentials

- 🎓 **B.S., Industrial & Systems Engineering**
- 📅 **University of Colorado Boulder** — graduate Data Structures & Algorithms pathway (MS-CS, 3 credits), from Nov 2026
- 📅 **Georgia Tech OMSCS** — M.S. Computer Science (Computing Systems), applying Aug 2027
- 🧾 **Next exams:** Azure AI Fundamentals (AI-901) · Fabric Data Engineer (DP-700) · AWS Data Engineer – Associate — [full plan](https://github.com/manuel-reyes-ml/learning_journey#-credentials)

---

📫 [manuelreyesv410@gmail.com](mailto:manuelreyesv410@gmail.com) · [LinkedIn](https://www.linkedin.com/in/mr410/) · ♟️ chess player · 🌅 4:30 AM study routine, 25 hrs/week
