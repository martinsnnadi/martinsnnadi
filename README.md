# Martins Nnadi

**Data Engineer · United Kingdom**

I build data pipelines that survive contact with reality — the messy responses, the schema that changes without warning, the run that fails at 3am and has to recover on its own.

Currently a Data Engineering Intern on a Human-Centred AI research initiative, working across Azure Fabric, AWS and Snowflake. Before this, I spent nine years in oilfield operations, most recently as an Operations Manager, where I started building the reporting and analysis pipelines that eventually became the whole job.

That background shows up in how I work. Operations teaches you that a system nobody can maintain isn't finished, that the failure you didn't plan for is the one you'll get, and that documentation is not optional.

📍 United Kingdom · 💼 [LinkedIn](https://www.linkedin.com/in/nnadi-martins) · ✉️ martinsnnadi@yahoo.com

---

## What I work with

**Languages** · Python, SQL, PySpark
**Orchestration** · Apache Airflow, Astronomer Cosmos
**Warehousing** · Snowflake, PostgreSQL, Delta Lake, Microsoft Fabric
**Cloud** · AWS (S3, IAM), Microsoft Azure
**Transformation** · dbt, pandas, Spark window functions
**Formats & storage** · Parquet, JSON, VARIANT / semi-structured data
**Practice** · Medallion architecture, star schemas, dimensional modelling, Git and PR-based collaboration, Docker Compose

---

## Featured projects

Two pipelines built against the same public API, using deliberately opposite architectures. Together they're an argument about *when* each pattern is the right one.

### 🔵 [FPL ELT Pipeline — S3, Snowflake and dbt](https://github.com/martinsnnadi/de-fpl-elt-snowflake-dbt)

Raw JSON lands in S3. Snowflake reads it in place through external tables, with no copy. dbt builds Bronze → Silver → Gold, ending in a tested star schema of four dimensions and two facts.

Python performs no transformation whatsoever — the entire modelling layer is version-controlled SQL. Includes two Airflow DAG variants, one running dbt as a single task and one rendering an Airflow task per dbt model, because that choice is a genuine trade-off rather than a preference.

`Snowflake` `dbt` `S3` `Airflow` `Cosmos` `medallion architecture` `star schema`

### 🟢 [FPL ETL Pipeline — Airflow, S3 and Postgres](https://github.com/martinsnnadi/de-fpl-etl-airflow-postgres)

The same source, transformed in pandas before it reaches the warehouse, then written to two destinations: Parquet in the data lake and query-ready tables in Postgres.

The DAG is deliberately thin — it defines task order and nothing else. All logic sits in an importable package that unit tests exercise in milliseconds without a scheduler running. Audit columns on every table, nested columns dropped defensively, no credentials anywhere in code.

`Python` `pandas` `Airflow` `PostgreSQL` `MinIO / S3` `Parquet` `pytest`

---

## Current work

**Human-Centred AI Research Initiative** — Data Engineering Intern *(May 2026 – present)*

- Built an Azure Fabric medallion lakehouse processing 10.6M+ OULAD clickstream records from Bronze through to Gold
- Developed PySpark transformations using window functions to turn asynchronous interaction logs into weekly learner-behaviour features
- Implemented column-level masking and salted SHA-256 tokenisation to protect sensitive identifiers in flight
- Engineered an Airflow-based AWS ingestion workflow for high-frequency WESAD physiological data, using stream-unzip parsing to avoid memory bottlenecks on large archives
- Integrated multi-year NHANES health datasets into Snowflake with dbt-based data-quality testing, applying survey weighting and explicit missing-data strategies

---

## Certifications

Microsoft Certified: Fabric Data Engineer Associate (DP-600) · Microsoft Certified: Azure Data Fundamentals (DP-900) · Python Essentials 1 · Data Analytics Essentials · ISO 9001:2015 Internal Auditor

---

## Background

**Pgd, Computer Science** — University of Port Harcourt
**BSc, Industrial Physics** — Federal University of Agriculture, Makurdi

Nine years across oilfield operations and data analysis before moving into engineering full-time — leading field teams, building the reporting that made those decisions evidence-based, and learning what happens to a system when the person who built it is unavailable.

---

## Open to

Data Engineering roles in the UK. Particularly interested in teams working on warehouse modernisation, orchestration at scale, or data quality and governance.

**[LinkedIn](https://www.linkedin.com/in/nnadi-martins)** · **martinsnnadi@yahoo.com**
