<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=180&section=header&text=Ashish%20Patel&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Data%20Engineer%20%7C%20Data%20Analyst%20%7C%20Software%20Engineer&descAlignY=58&descSize=18&descColor=a8d8ea&animation=fadeIn" width="100%"/>

[![Portfolio](https://img.shields.io/badge/Portfolio-16302b?style=flat-square&logo=vercel&logoColor=white)](https://ashishpatelde.vercel.app)
&nbsp;
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ashish-patel-39b50b292/)
&nbsp;
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:ashishpatelap1403@gmail.com)
&nbsp;
[![SDSU MS Big Data Analytics — GPA 4.0](https://img.shields.io/badge/SDSU_MS_Big_Data_Analytics-GPA_4.0-CC0033?style=flat-square)](https://www.sdsu.edu)

</div>

---

Data engineer with **4 years of industry experience** across the full path data takes — batch and near-real-time ingestion in Python, PySpark and Kafka, modeled with dbt in Snowflake and Delta Lake, orchestrated in Airflow, and surfaced through Power BI, Tableau and Streamlit.

Two things shape how I work. First, **data quality is not a downstream problem** — Great Expectations suites, dbt tests and OpenLineage tracking mean schema drift surfaces at ingest rather than three dashboards later. Second, **a pipeline is only worth what someone does with it**, which is why I spend as much time on the reporting and application layer as on the ingestion side.

I hold an **MS in Big Data Analytics** from San Diego State (GPA 4.0) and I'm open to data engineer, data analyst and software engineer roles.

---

## Experience

**Data Engineer — Digit Insurance** *(Jun 2022 – Jul 2024)*

Engineered batch and near-real-time ETL/ELT pipelines in Python, SQL, PySpark and Kafka, integrating claims, policy, billing and REST API sources across **10M+ insurance records** into a centralized Databricks lakehouse. Built Delta Lake medallion workflows on incremental merge patterns instead of full reloads, improving processing efficiency by **25%** and lowering daily cluster cost. Modeled claims, billing and policy domains in Snowflake with dbt, cutting data retrieval time by **50%** for underwriting and finance reporting.

On the reporting side, I automated recurring claims and finance reporting in partnership with claims operations — eliminating **100+ hours of manual work per month** and delivering the daily curated SLA dataset behind within-SLA claim settlement rising from **65% to 95%**.

**Graduate Data Engineer — San Diego State University** *(Sep 2024 – May 2026)*

Designed an AWS S3 research data lake with raw and curated zones, consolidating four heterogeneous source types — telemetry, mission logs, REST APIs and geospatial — into one governed dataset. Built reusable Python, PySpark and SQL ingestion and schema-normalization pipelines that cut downstream data-quality defects by **40%**, backed by Great Expectations validation suites and Marquez/OpenLineage lineage tracking. Tuned Spark jobs through partitioning, caching and a Parquet layout redesign, and delivered self-serve Streamlit dashboards that reduced research staff preparation and reporting time by **80%**.

---

## Projects

### Data & Analytics Engineering

**[Snowflake · dbt · Airflow Pipeline](https://github.com/AshishPatel14S/snowflake-dbt-airflow-data-pipeline)** — `Snowflake` `dbt` `Airflow` `Astronomer Cosmos` `AWS S3` `Docker`

S3-to-Snowflake ELT pipeline for Airbnb booking, listing and host data, orchestrated as Airflow DAGs via Astronomer Cosmos on a containerized Docker deployment. Eight dbt models and three SCD Type 2 snapshots with validation tests produce history-tracked dimensional and OBT outputs for repeatable daily refreshes.

**[SaaS Revenue Data Platform](https://github.com/AshishPatel14S/saas-revenue-analytics-databricks-dbt)** — `Databricks` `dbt` `Unity Catalog` `SQL` `Python`

Databricks and dbt medallion platform over 8 SaaS source tables spanning customers, subscriptions, invoices, payments, product usage and support. Nine Gold-layer marts cover MRR, churn and reactivation, billing collections, engagement and Customer 360 — enforced by dbt uniqueness, relationship, accepted-value and MRR reconciliation tests.

**[Health Sensing Data Pipeline](https://github.com/AshishPatel14S/health-sensing-data-pipeline)** — `Python` `Pandas` `PyArrow` `Parquet` `unittest`

Turns raw JSON event logs into analytics-ready Parquet: validates required fields, logs and discards malformed events so a bad row can't halt the run, flattens nested metadata to avoid downstream joins, and normalizes timestamps to UTC. Unit tests cover extraction, transformation and aggregation, including empty and malformed inputs.

---

### Analytics & Experimentation

**[Airline Operations Intelligence](https://github.com/AshishPatel14S/airline-ops-intelligence)** — `PostgreSQL` `SQL` `Power BI` `DAX` `Star Schema`

Across **8.4M BTS domestic flight records** and 17 U.S. carriers, **76.5% of all delay minutes turn out to be operationally controllable** — carrier issues (37%) and late-aircraft propagation (39.4%) dwarf weather and NAS combined, and the gap between best and worst carrier OTP is 16.9 percentage points. Built on a star schema with CTEs, window functions and CASE-based delay attribution, delivered as a two-page Power BI executive dashboard.

**[A/B Test Analysis Framework](https://github.com/AshishPatel14S/A-B-Test-Analysis)** — `Python` `SciPy` `Statsmodels` `Bayesian Inference`

Checkout experiment across 100K randomized users measuring a **+1.95pp conversion lift** (10.84% → 12.79%) at p < 0.001, 95% CI [1.55pp, 2.35pp], with an estimated ~$9.9M annualized revenue impact. Reusable framework covering SRM checks, power analysis, chi-square and z-test validation, and segmentation by device and user type.

**[E-Commerce Sales Dashboard](https://github.com/AshishPatel14S/ecommerce-sales-dashboard)** — `Python` `Pandas` `Plotly` `Streamlit` `RFM` `Cohort Analysis`

Cleaned 1.07M raw transactions down to 541K quality records across 5,942 customers in 38 countries, then built RFM segmentation and cohort retention views. Surfaced a **3× November revenue spike** and the finding that the **top 20% of customers generate 78% of revenue** — directly actionable for inventory planning and retention targeting.

---

### Software & AI Engineering

**[CureMatch](https://github.com/AshishPatel14S/curematchh)** — `Next.js 14` `TypeScript` `SQLite` `Python` `Llama 3.3 70B` `LoRA`

Clinical trial matching across **65,081 actively recruiting ClinicalTrials.gov studies**. A rule-based parser extracts excluded medications, lab thresholds and ECOG ranges into a derived database; a deterministic engine scores a patient profile on six weighted criteria in milliseconds. The LLM narrates verdicts and answers grounded questions but never touches the matching decision, so every exclusion traces back to a rule.

**[CaseRoom](https://github.com/AshishPatel14S/Caseroom)** — `FastAPI` `LangGraph` `Qdrant` `Supabase` `Redis` `Next.js` `Stripe` `Docker`

Adaptive USMLE study platform generating clinical cases through an 8-node LangGraph pipeline with a validator node that loops back on clinical errors. RAG over a Qdrant medical knowledge base grounds each vignette; a six-level mastery model across 76 topics routes the next case toward the student's weakest areas. Redis pre-generation runs the next case in the background so it lands instantly.

---

## Skills

| | |
|---|---|
| **Programming** | Python (Pandas, NumPy, PySpark), SQL, TypeScript, R, Bash, CTEs, Window Functions |
| **Data Engineering** | Apache Spark, Databricks, Kafka, Airflow, dbt, ETL/ELT, Incremental Loads |
| **Cloud & Lakehouse** | AWS S3, Azure Data Factory, Azure Data Lake, Azure Synapse, Snowflake, Delta Lake, Unity Catalog, Medallion Architecture |
| **Warehousing & Modeling** | PostgreSQL, MySQL, BigQuery, Dimensional Modeling, Star Schema, Data Marts, Query Optimization |
| **Data Quality & DevOps** | Great Expectations, Marquez/OpenLineage, dbt Tests, Profiling, Git, Docker, CI/CD |
| **Analytics & BI** | Power BI, DAX, Power Query, Tableau, Streamlit, Excel, A/B Testing, RFM, Cohort Analysis |
| **Applications** | FastAPI, Next.js, React, Supabase, Redis, LangGraph, RAG, Qdrant |

---

## Education

**MS, Big Data Analytics** — San Diego State University *(May 2026, GPA 4.0)*
Coursework: ML Engineering, Data Mining, Enterprise Database Management, GIS Programming, Reinforcement Learning, Big Data Tools & Methods

**Certifications:** CS50's Introduction to Python (Harvard) · Google Data Analytics Professional Certificate

---

<div align="center">

*Open to full-time data engineer, data analyst and software engineer roles — onsite or remote*

[![Portfolio](https://img.shields.io/badge/See_the_full_portfolio-16302b?style=for-the-badge&logo=vercel&logoColor=white)](https://ashishpatelde.vercel.app)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer" width="100%"/>

</div>
