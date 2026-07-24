# Hi, I'm Manuel 👋

![Production AI](https://img.shields.io/badge/🤖_Production_AI_&_Data_Systems-AI--Focused_Data_Engineering_·_Applied_AI-blueviolet?style=for-the-badge)

**Production AI & data systems — AI-Focused Data Engineering · Analytics Engineering · Applied AI** | Eval-first · measurable outcomes · proof over keywords

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?logo=linkedin)](https://www.linkedin.com/in/mr410/)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?logo=gmail)](mailto:manuelreyesv410@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-Projects-667eea)](https://github.com/manuel-reyes-ml/data-portfolio)
[![Roadmap](https://img.shields.io/badge/Roadmap-v10.0-28a745)](https://manuel-reyes-ml.github.io/learning_journey/roadmap.html)

---

## 🎯 What I'm Building Right Now

- 🏗️ **PolicyPulse** — RAG → GraphRAG chatbot over retirement-plan documents, with **blocking eval gates** (RAGAS/DeepEval) and a **FastMCP server**. *(Applied-AI flagship)*
- 🧾 **1099 Data Platform** — hardening a **live** financial ETL system into a full data platform: dbt-tested models, orchestration, data contracts, containerized deploy. *(Data Engineering flagship)*
- 📜 **Employer AI track** — Azure AI Fundamentals (AI-901) → AI Agent Builder Associate (AB-620), building internal automations on the Microsoft/Copilot stack.

**Where I am → where I'm headed:** Currently an **Internal AI Builder** (current stage). **Next goal:** **AI-Focused Data Engineer / Analytics Engineer** — building AI-aligned, AI-managed data pipelines, not vanilla DE. **After that:** **Applied AI Engineer** (as part of a Forward-Deployed Engineer / FDE track).

---

## 💼 What Makes Me Different

My focus is **proof over keywords**: production systems with evaluation gates and measurable business impact — across data engineering and applied AI. Deep domain knowledge (including regulated finance) is an edge I bring, not the boundary of where I work.

| Most Candidates | What I Bring |
|:----------------|:-------------|
| 🎓 Tutorial projects (Titanic, taxi data) | ✅ **Live production ETL** at a financial firm — caught **450+ incorrect tax codes** before participants received bad documents |
| ❌ No domain expertise | ✅ **15+ yrs business operations** (manufacturing, digital marketing) · **2 yrs ERISA-regulated financial operations** · **5+ yrs independent trading** |
| 📦 Ten shallow repos | ✅ **Focused portfolio: 3 flagships + 2 supporting** — real systems, not a repo pile |
| 🤖 "Prompts ChatGPT" | ✅ **Production AI**: Anthropic SDK primary, RAG + **GraphRAG (Neo4j)**, **FastMCP server**, Pydantic structured outputs, privacy-routed local models (Ollama/LM Studio) |
| 📉 No evaluation | ✅ **Eval-first, blocking gates** (DeepEval/RAGAS/GEval, faithfulness ≥ 0.9) — the discipline that separates prototypes from production systems |
| 🧰 Notebooks & one-off scripts | ✅ **Production engineering**: typed Python, **`uv` + committed `uv.lock`** (reproducible by construction), `pyproject.toml` + `src/`, ruff/mypy, Docker, GitHub Actions CI, Conventional Commits |
| 🗣️ Pure coding-interview prep | ✅ **FDE discovery & decomposition edge** — the customer-facing case-study round that filters most technically-strong candidates; **2 yrs ERISA client-facing operations** is the structural advantage, and every flagship carries an ADR set + C4 diagram to defend the design |

---

## 🚀 Production Highlight — the live core of the DE flagship

### 🧾 [1099 Reconciliation ETL Pipeline](https://github.com/manuel-reyes-ml/1099_reconciliation_pipeline)
**Status:** ✅ Live in production | 🌐 Public repository

Automated Python ETL for retirement-plan distribution reconciliation at Daybright Financial — the live system now being production-hardened into the **1099 Data Platform** (Data Engineering flagship).

| Metric | Impact |
|--------|--------|
| ⚡ Time Saved | **95% reduction** (4–6 hours → 15 min/week) |
| 💰 Cost Savings | **$15,000+/year** in labor |
| 📊 Scalability | **10x capacity** (300+ accounts vs 30 manual) |
| ✅ Accuracy | **Zero errors** since deployment |

**Tech:** Python • pandas • openpyxl • matplotlib • data validation • pytest • GitHub Actions CI • faker (synthetic data)

**[→ View Documentation & Code](https://github.com/manuel-reyes-ml/1099_reconciliation_pipeline)**

---

## 🏆 Portfolio — 3 Flagships + 2 Supporting

> A deliberately focused portfolio — a few substantial systems, each targeting a different problem: Applied AI, Data Engineering, and autonomous-systems safety.
>
> 🏗️ **Production standard (every repo):** architecture diagram (Mermaid) • **ADR set (`docs/adr/`) + C4 context diagram** • Dockerfile • evaluation-metrics table • 15–30s demo GIF • "What I Learned." **Standards, non-negotiable:** no vibe coding (every line understood before merge) • eval-first blocking gates • **synthetic data only** in public repos • `pyproject.toml` + **`uv.lock`** + `src/` + `py.typed` + ruff + mypy • Conventional Commits • **uv-managed environments** (`uv sync --frozen` in CI/Docker; no `requirements.txt`).

### 🏁 Flagship 1 — [PolicyPulse](https://github.com/manuel-reyes-ml/policypulse) · *Applied-AI*
**RAG → GraphRAG document intelligence** | 🔌 Exposes a **FastMCP server**

Answers retirement-plan policy questions with cited sources, auto-escalates when uncertain, and enforces **per-document access control at retrieval time** — a differentiator for sensitive-document use cases.

| Dimension | Implementation |
|-----------|----------------|
| 🔍 Retrieval | Embeddings + **ChromaDB**; **GraphRAG hybrid (Neo4j + ChromaDB)** for multi-hop questions |
| 📎 Grounding | Every answer cites specific policy section & document |
| 🎫 Escalation | Confidence gate → auto-generated ticket with context |
| 🔌 MCP | FastMCP exposes retrieval as MCP tools (Cursor / Claude Desktop) |
| 🧪 Evaluation | **RAGAS + DeepEval as blocking gates**; access-control-aware retrieval |

**Tech:** Python • **Anthropic SDK (primary, Gemini fallback)** • ChromaDB • **Neo4j (GraphRAG)** • Gemini Embeddings • Streamlit • Pydantic • DeepEval • RAGAS • **FastMCP** • Docker • GitHub Actions CI

---

### 🏁 Flagship 2 — [1099 Data Platform](https://github.com/manuel-reyes-ml/1099_reconciliation_pipeline) · *Data Engineering*
**Production financial data platform** — the live 1099 pipeline (above), hardened end-to-end

Ingestion → **dbt-tested models (CI-gated)** → **orchestrated (Airflow)** → **data-quality contracts** → **deployed (Docker/ECS)** → **monitored**, with written incident/postmortems. Adds a **semantic / metrics layer** for the Analytics-Engineer story, plus an **S3 DataVault Applied-AI layer** (NL-to-SQL over the semantic layer, HITL on every write).

| Layer | Implementation |
|-------|----------------|
| 🔄 Transformation | **dbt** — tested models at real scale, docs alongside code, CI that gates merges |
| 🗓️ Orchestration | **Airflow** DAGs with retries, alerting, monitoring |
| 🛡️ Quality & governance | Data contracts, **dbt tests / Great Expectations**, lineage, access-control awareness |
| 📦 Deploy & ops | **Docker → ECS/Fargate**, Terraform basics, incident writeups |
| 📊 Semantic layer | Metric definitions + dashboard handoff (Power BI) — the AE differentiator |

**Tech:** Python • SQL • **dbt** • **Airflow** • **Snowflake** (primary warehouse) • BigQuery/Fabric awareness • DuckDB • Parquet • **Great Expectations** • Docker • **AWS (S3, ECS)** • **Terraform** • GitHub Actions CI

**Retains scheduling priority** — it feeds the first external move.

---

### 🏁 Flagship 3 — [Crucible](https://github.com/manuel-reyes-ml/crucible) · *Autonomous Execution Research* | 🦙 Local-First AI
**Backtest → paper → live** autonomous **multi-timeframe (swing → intraday)** research platform *(swing-first is the lower-risk on-ramp; intraday plugins follow once swing clears all three gates)*

Production-safety engineering for an autonomous system handling irreversible actions: a **mandatory human-in-the-loop sign-off + kill-switch** on the live path, and an **"LLM behind the Wall"** information barrier — the model sees only in-sample aggregated stats, never raw ticker-date outcomes. A **verifier agent** sits before the human gate. Grounded in 5+ years of hands-on independent trading.

| Dimension | Implementation |
|-----------|----------------|
| 🔒 Integrity | Sealed out-of-sample vault, logged overfitting budget, walk-forward CV |
| 🛡️ AI safety | LLM behind the Wall (aggregates only); deterministic core owns every trade; kill-switch on live path |
| ✅ Verification | Verifier-agent layer **before** the human sign-off gate |
| 📏 Agentic evals | **Tool Correctness = 1.0** (deterministic) · **Task Completion > 0.8** (judged), published |
| 🔌 Plugins | Strategies are plugins (Protocol + ABC + registry); IT-1 ORB + VWAP Reclaim prove the abstraction |

**Tech:** Python • own event-driven backtest harness → **NautilusTrader** • Optuna • DuckDB • Parquet • **Ollama/Qwen3 (local-first)** → Anthropic/Gemini • Pydantic • **LangGraph** • **Alpaca** + **Schwab/TOS** • DeepEval • Docker • GitHub Actions CI • **uv** *(Conda conditional — only if compiled/GPU backends land)*

> ⚖️ *Educational/research project. Not investment advice; makes no claim of positive expectancy — validation is the entire point.*

---

### 🧩 Supporting — [FormSense](https://github.com/manuel-reyes-ml/formsense) · *Document AI*
Multimodal **agentic workflow** (Anthropic *Building Effective Agents* taxonomy — precise vocabulary, *not* multi-agent) that extracts and validates synthetic ERISA distribution forms against a frozen Pydantic schema contract, with **GEval schema-adherence** gates and smart routing.

**Tech:** Python • Vision LLM • Streamlit • Pydantic • DeepEval (GEval) • Docker • GitHub Actions CI

### 🧩 Supporting — [Attention-Flow Catalyst (AFC)](https://github.com/manuel-reyes-ml/attention-flow-catalyst) · *Research*
Read-only **GraphRAG** financial-research loop over small-cap trigger signals, with a **faithfulness ≥ 0.9** evaluation showcase (financial-data sensitivity). Demonstrates bounded, unattended-safe agent design. *The eval-first faithfulness benchmark ships in S1 → S3.*

**Tech:** Python • DuckDB • Parquet • edgartools • **Neo4j + ChromaDB (GraphRAG)** • **Anthropic SDK** • DeepEval • SelfCheckGPT + FActScore • Docker • CI

---

### 📅 Backlog (production-grade when built)
- 📊 **[Operations-Demand-Intelligence](https://github.com/manuel-reyes-ml/operations-demand-intelligence)** — workflow-demand analytics on enterprise OnBase data for data-driven staffing (consolidation candidate against the 1099 platform's mart/AI layer).
- 📺 **[StreamSmart Optimizer](https://github.com/manuel-reyes-ml/streamsmart-optimizer)** — consumer AI app (external APIs, async HTTP, rotation/cost optimization).

> The former standalone **DataVault Analyst** (PandasAI / NL querying) is now the **S3 Applied-AI layer of Flagship 2** — text-to-SQL over the semantic layer, HITL on every write. No separate repo.

---

## 📌 Repository Guide

| Type | Repository | Description |
|------|------------|-------------|
| 🏁 **Flagship — Applied AI** | [policypulse](https://github.com/manuel-reyes-ml/policypulse) | RAG → GraphRAG + FastMCP + access-control retrieval |
| 🏁 **Flagship — Data Eng** | [1099_reconciliation_pipeline](https://github.com/manuel-reyes-ml/1099_reconciliation_pipeline) | Live ETL → production data platform (dbt/Airflow/contracts) |
| 🏁 **Flagship — Autonomous** | [crucible](https://github.com/manuel-reyes-ml/crucible) | Backtest→paper→live; HITL + kill-switch + LLM-behind-the-Wall |
| 🧩 **Supporting — Doc AI** | [formsense](https://github.com/manuel-reyes-ml/formsense) | Multimodal agentic-workflow form extraction & validation |
| 🧩 **Supporting — Research** | [attention-flow-catalyst](https://github.com/manuel-reyes-ml/attention-flow-catalyst) | Read-only GraphRAG financial research (faithfulness ≥ 0.9) |
| 📅 **Backlog** | [operations-demand-intelligence](https://github.com/manuel-reyes-ml/operations-demand-intelligence) | Workflow-demand analytics |
| 📅 **Backlog** | [streamsmart-optimizer](https://github.com/manuel-reyes-ml/streamsmart-optimizer) | Consumer AI (API integration, async) |
| 📖 Journey | [learning_journey](https://github.com/manuel-reyes-ml/learning_journey) | Public documentation & roadmap |

📚 [Data Portfolio Hub](https://github.com/manuel-reyes-ml/data-portfolio) — central index with business context, technical details, and impact metrics.

---

## 🛠️ Technical Skills

**Languages & Dev Tools**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![Cursor](https://img.shields.io/badge/Cursor_AI-000000?style=flat-square&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Bash](https://img.shields.io/badge/Bash/CLI-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Makefile](https://img.shields.io/badge/Makefile-A42E2B?style=flat-square&logo=gnu&logoColor=white)
![uv](https://img.shields.io/badge/uv_(Astral)-DE5FE9?style=flat-square&logo=uv&logoColor=white)
![Anaconda](https://img.shields.io/badge/Conda-conditional-44A833?style=flat-square&logo=anaconda&logoColor=white)

**Data Analysis & Processing**

![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![Parquet](https://img.shields.io/badge/Parquet-50ABF1?style=flat-square&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=flat-square&logo=googlesheets&logoColor=white)

**Data Engineering / Analytics Engineering** 🆕 *Stage 2 build*

![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![Airflow](https://img.shields.io/badge/Apache_Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=flat-square&logo=googlebigquery&logoColor=white)
![Microsoft Fabric](https://img.shields.io/badge/Microsoft_Fabric-0078D4?style=flat-square&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Great Expectations](https://img.shields.io/badge/Great_Expectations-FF6310?style=flat-square&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_(S3/Redshift/Glue)-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)

**Visualization & BI**

![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat-square&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)

**Testing, CI/CD & Containerization**

![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![ruff](https://img.shields.io/badge/ruff-D7FF64?style=flat-square&logo=ruff&logoColor=black)
![uv](https://img.shields.io/badge/uv_sync_--frozen-DE5FE9?style=flat-square&logo=uv&logoColor=white)
![mypy](https://img.shields.io/badge/mypy-2A6DB2?style=flat-square&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)

**AI & GenAI**

![Anthropic SDK](https://img.shields.io/badge/Anthropic_SDK_(primary)-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Gemini SDK](https://img.shields.io/badge/Gemini_SDK-8E75B2?style=flat-square&logo=google&logoColor=white)
![OpenAI API](https://img.shields.io/badge/OpenAI_API-412991?style=flat-square&logo=openai&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama_(local--first)-000000?style=flat-square&logo=ollama&logoColor=white)
![LM Studio](https://img.shields.io/badge/LM_Studio_(local)-4A154B?style=flat-square&logoColor=white)
![Qwen3](https://img.shields.io/badge/Qwen3_(local)-615CED?style=flat-square&logoColor=white)
![FastMCP](https://img.shields.io/badge/FastMCP-7C3AED?style=flat-square&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logoColor=white)
![OpenCode](https://img.shields.io/badge/OpenCode_(agentic_harness)-000000?style=flat-square&logoColor=white)
![PandasAI](https://img.shields.io/badge/PandasAI-150458?style=flat-square&logo=pandas&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F61?style=flat-square&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j_(GraphRAG)-008CC1?style=flat-square&logo=neo4j&logoColor=white)

**AI Evaluation**

![DeepEval](https://img.shields.io/badge/DeepEval-FF6B6B?style=flat-square&logoColor=white)
![RAGAS](https://img.shields.io/badge/RAGAS-4CAF50?style=flat-square&logoColor=white)
![GEval](https://img.shields.io/badge/GEval-9C27B0?style=flat-square&logoColor=white)
![SelfCheckGPT](https://img.shields.io/badge/SelfCheckGPT-FF9800?style=flat-square&logoColor=white)
![FActScore](https://img.shields.io/badge/FActScore-00897B?style=flat-square&logoColor=white)
![LangSmith](https://img.shields.io/badge/LangSmith-1C3C3C?style=flat-square&logoColor=white)

**Trading & Backtesting (Crucible / AFC)**

![NautilusTrader](https://img.shields.io/badge/NautilusTrader-00BFA5?style=flat-square&logoColor=white)
![Optuna](https://img.shields.io/badge/Optuna-2196F3?style=flat-square&logo=optuna&logoColor=white)
![Alpaca](https://img.shields.io/badge/Alpaca_API-FFD400?style=flat-square&logoColor=black)
![Schwab](https://img.shields.io/badge/Schwab_Trader_API-009DDC?style=flat-square&logoColor=white)
![edgartools](https://img.shields.io/badge/edgartools_(SEC)-002868?style=flat-square&logoColor=white)
![yfinance](https://img.shields.io/badge/yfinance-7B1FA2?style=flat-square&logoColor=white)

**Domain Expertise:** 15+ years business operations (manufacturing, digital marketing) • 2 years ERISA-regulated financial operations (retirement plans) • 5+ years independent trading (fuels the research flagships)

---

## 🗺️ The Path — 3 Stages · ~32 Months · Evidence-First

*Immediate focus: production automations and AI-builder scope at my current employer, while the engineering foundation and Flagship #1 ship in parallel.*

| Stage | Timeline | Role / Goal | Status |
|-------|----------|-------------|--------|
| **1** | Months 1–8 | **Internal AI Builder** (current employer, no comp reset) | 🟢 **ACTIVE** |
| **2** | Months 9–20 | **AI-Focused Data Engineer / Analytics Engineer** (dual-target) | ⚪ Planned |
| **3** | Months 21–32 | **Applied AI Engineer → FDE track** | 🎯 Goal |

> **Fallback logic:** if internal elevation produces no scope change by Month 8, the external **Data Engineer / Analytics Engineer** search opens at Month 10–12 — not a Data Analyst search.

**[→ View Interactive Roadmap (v10.0)](https://manuel-reyes-ml.github.io/learning_journey/roadmap.html)**

---

## 🎓 Education & Certifications

### Certification stack — *replace, not stack* (each credential serves a named purpose)

| Cert | Track | Stage |
|------|-------|-------|
| ![AI-901](https://img.shields.io/badge/Azure_AI_Fundamentals-AI--901-0078D4?style=flat-square&logo=microsoftazure&logoColor=white) | Employer (reimbursed) | S1 |
| ![AB-620](https://img.shields.io/badge/AI_Agent_Builder_Assoc-AB--620-0078D4?style=flat-square&logo=microsoftazure&logoColor=white) | Employer (reimbursed) | S1–S2 |
| ![DP-700](https://img.shields.io/badge/Fabric_Data_Engineer-DP--700-0078D4?style=flat-square&logo=microsoftazure&logoColor=white) | Employer (reimbursed) | S2 |
| ![AWS DEA](https://img.shields.io/badge/AWS_Data_Engineer-Associate-232F3E?style=flat-square&logo=amazonaws&logoColor=white) | Personal | S2 |
| ![NCA-GENL](https://img.shields.io/badge/NVIDIA-NCA--GENL-76B900?style=flat-square&logo=nvidia&logoColor=white) | Personal | S3 |
| ![Databricks](https://img.shields.io/badge/Databricks-GenAI_Engineer_Assoc-FF3621?style=flat-square&logo=databricks&logoColor=white) | Personal | S3 |
| ![Neo4j](https://img.shields.io/badge/Neo4j-Certified_Professional-008CC1?style=flat-square&logo=neo4j&logoColor=white) | Personal | S3 |
| ![AI-103](https://img.shields.io/badge/Azure_AI_Apps_&_Agents_Dev-AI--103-0078D4?style=flat-square&logo=microsoftazure&logoColor=white) | Employer (reimbursed) | S3 |
| ![CCA-F](https://img.shields.io/badge/Anthropic-CCA--F-D97757?style=flat-square&logo=anthropic&logoColor=white) | Personal | S3 |
| ![dbt AE](https://img.shields.io/badge/dbt_Analytics_Engineering-conditional-FF694B?style=flat-square&logo=dbt&logoColor=white) | Personal *(if AE apps stall)* | S2 |

> **AI-103** (code-first Azure/Foundry — Python, agentic + RAG) is the employer-reimbursable mirror of **CCA-F**: AB-620 is the low-code Copilot Studio maker path, AI-103 the code-first developer path.
> *Conditional platform-cert menu (take **ONE**, matched to a target employer's stack — never stacked): lakehouse slot — **DP-750** (Azure Databricks, reimbursed) preferred / SnowPro Core (COF-C03) / Databricks DE fallback.*

### Coursework credentials (Coursera Professional Certificates)
- 🚧 **IBM Generative AI Engineering Professional Certificate** (16 courses) — *Stage 1 spine*: RAG, LangChain, fine-tuning, deployment
- 📅 **AWS Data Engineering Professional Certificate** — *Stage 2 DE spine*: S3, Redshift, Glue, EMR, Kinesis

### Active learning (Stage 1)
- 🚧 **CS50: Introduction to Computer Science** (Harvard) — CS fundamentals + OMSCS admission evidence
- 🚧 **Python for Everybody** (U. Michigan) • **AI Python for Beginners** (DeepLearning.AI)
- 🚧 **Building with the Claude API** (Anthropic Academy) — official SDK source-of-truth
- 🚧 **Improving Accuracy of LLM Applications** + **Building & Evaluating Advanced RAG** (DeepLearning.AI) — eval-driven development
- 🚧 **MCP: Build Rich-Context AI Apps with Anthropic** (primer) • **AI Prompting for Everyone** • **30 Days of Streamlit** • **Docker for Beginners** (KodeKloud)
- 🚧 **uv — Python packaging & environments** ([Astral official docs](https://docs.astral.sh/uv/) + [Al Sweigart's quickstart](https://inventwithpython.com/blog/uv-quickstart-tutorial.html)) — the tool every repo now builds on
- ⏸️ *Conditional:* **Conda Basics** (Anaconda Learning) — reserved for Crucible **only if** it grows compiled numerical / CUDA / BLAS backends
- ⭐ *Elective:* **Statistics with Python** (U. Michigan) — inferential module feeds eval statistics

### 🎓 Degree (parallel track)
- 📅 **Georgia Tech OMSCS** — M.S. Computer Science, **Computing Systems** specialization (distributed systems, databases, OS, architecture). Mapped to Stages 2–3 as a substitute for redundant self-study; AI/ML electives substitute for the ML-literacy module. *Academic projects kept separate from public repos.*

---

## ⚡ Quick Facts

- 🧾 **Live production system** in a regulated financial domain — with evaluation gates, not vibes
- 🏰 **Finance/ERISA + trading domain depth** — 2 yrs ERISA-regulated operations + 5+ yrs independent trading
- 🌅 **4:30 AM club** (early-morning focused study)
- ♟️ **Chess player** (strategy translates to systems)
- 🤖 Fascinated by **LLMs transforming financial analysis** — behind eval gates and safety barriers
- 📚 Reading: *Machine Learning for Algorithmic Trading* • *Hands-On LLMs* • *Building Effective Agents* (Anthropic)
- ⚡ **Reproducible by default** — uv-managed environments with committed lockfiles across every repo
- 🎯 Obsessed with **data-driven decisions** and **proof over keywords**

---

## 📊 GitHub Activity

<div align="center">

### 📈 Stats & Contributions

<div align="center">
  <img src="https://github-readme-stats-theta-three-33.vercel.app/api?username=manuel-reyes-ml&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" height="165" alt="github stats" />
  <img src="https://streak-stats.demolab.com?user=manuel-reyes-ml&theme=tokyonight&hide_border=true" height="165" alt="streak stats" />
</div>

### 💻 Most Used Languages

![Top Languages](https://github-readme-stats-theta-three-33.vercel.app/api/top-langs/?username=manuel-reyes-ml&layout=compact&theme=tokyonight&hide_border=true&langs_count=8)

</div>

---

## 🌐 Let's Connect

**Open to:**
- 💼 **Data Engineer / Analytics Engineer** roles (dual-target; AE more remote-accessible) — and **Applied AI / Forward-Deployed Engineer** roles across industries
- 🤝 Code reviews and technical discussions
- 🎓 Knowledge exchange on data + AI + finance

**Connect if you:**
- Value production code and evaluation evidence over tutorial completions
- Value domain depth and production controls (regulated/fintech a bonus, not a requirement)
- Are building **AI-ready data infrastructure** or **applied-AI systems** that must be trusted in production

---

<div align="center">

**Current Stage:** Internal AI Builder (Stage 1 of 3) | 🟢 Active • Building in Public • Evidence-First

⭐️ **Star repos** if useful • 🔔 **Follow** for updates on the ~32-month journey

</div>

<details>
<summary><b>💭 Building in Public — why</b> (click to expand)</summary>
<br>

I've worked with data my whole career — manufacturing, digital marketing, financial-plan operations, and years of independent trading. One truth kept repeating: **data-driven decisions beat intuition.** I hit a ceiling — I could analyze data well but couldn't build the automated systems to scale insight. So I'm building them, publicly.

- ✅ **Transparency:** real learning is messy — I show process, not just polished results
- ✅ **Accountability:** public commits are public commitment
- ✅ **Evidence:** this profile *is* the proof of ability and trajectory

The bet isn't more certificates or broader titles — it's **proof**: production systems with evaluation gates, deployed and measured, with stories that stand up to scrutiny.

</details>
