# Martins Nnadi

**Data Engineer · United Kingdom**

I build data pipelines that survive contact with reality — the messy responses, the schema that changes without warning, the run that fails at 3am and has to recover on its own.

Currently a Data Engineering Intern on a Human-Centred AI research initiative, designing local-first, serverless data architectures using DuckDB and dbt Core. Before this, I spent nine years in oilfield operations, most recently as an Operations Manager, where I started building the reporting and analysis pipelines that eventually became the whole job.

That background shows up in how I work. Operations teaches you that a system nobody can maintain isn't finished, that the failure you didn't plan for is the one you'll get, and that documentation is not optional.

📍 United Kingdom · 💼 [LinkedIn](https://www.linkedin.com/in/nnadi-martins) · ✉️ martinsnnadi@yahoo.com

---

## What I work with

**Languages** · Python, SQL
**Orchestration** · Python scripting workflow engines
**Warehousing** · DuckDB local-first database instances, relational data warehouses
**Transformation** · dbt Core, SQL window functions, dataset downsampling, data type-casting overrides
**Formats & storage** · Fixed-width layout data (.dat), CSV, binary serialized python objects (.pkl), Parquet
**Practice** · Medallion architecture, star schemas, dimensional modelling, Human-in-the-Loop (HITL) curation gates, data governance outlier sanitisation, Git and version control

---

## Featured projects

Two production repositories utilizing distinct engine paradigms to process data. Together they demonstrate when to deploy cloud-based ELT warehouses versus local-first, serverless architectures with integrated human curation gates.

### 🔵 [hcai-duckdb-research-platform](https://github.com/martinsnnadi/hcai-duckdb-research-platform)

Heterogeneous streams land on a local workstation workstation. DuckDB processes raw data into a clean medallion structure, and dbt Core builds Staging → Silver → Gold, ending in 12 distinct, research-ready marts.

SQL transformations utilise complex window functions to extract longitudinal click-variance timelines, binarise clinical health phenotypes, and compute within-subject baseline Z-scores to normalise physiological sensor drift. Includes a Human-in-the-Loop (HITL) curation gate using DuckDB file scans and upstream exclusion joins to flag demographic fairness gaps, severe clinical outliers, and physical sensor dropouts.

`DuckDB` `dbt Core` `Python` `medallion architecture` `Human-in-the-Loop` `Hybrid Intelligence` `Data Governance`


### 🔵 [FPL ELT Pipeline — S3, Snowflake and dbt](https://github.com/martinsnnadi/de-fpl-elt-snowflake-dbt)

Raw JSON lands in S3. Snowflake reads it in place through external tables, with no copy. dbt builds Bronze → Silver → Gold, ending in a tested star schema of four dimensions and two facts.

Python performs no transformation whatsoever — the entire modelling layer is version-controlled SQL. Includes two Airflow DAG variants, one running dbt as a single task and one rendering an Airflow task per dbt model, because that choice is a genuine trade-off rather than a preference.

`Snowflake` `dbt` `S3` `Airflow` `Cosmos` `medallion architecture` `star schema`

---

## Current work

**Human-Centred AI Research Initiative** — Data Engineering Intern *(May 2026 – present)*

- Built a local serverless medallion architecture using DuckDB and dbt Core to process over 10.6M OULAD clickstream records from raw ingestion through to 12 research-ready Gold mart tables.
- Developed high-performance SQL window functions to transform asynchronous student logs into longitudinal weekly learner-behaviour features and click-variance indicators.
- Implemented salted SHA-256 cryptographic masking within final database transformation schemas to permanently secure sensitive participant identifiers for Section 4 privacy compliance.
- Engineered a free, memory-efficient Python ingestion buffer to process multi-gigabyte WESAD binary pickle files natively on disk, downsampling high-frequency streams to a stable 1Hz research standard.
- Harmonised multi-source fixed-width NHANES datasets via a protective relational LEFT JOIN model to isolate an absolute baseline of 18,162 records while deploying automated dbt Core data-quality schema testing and missingness density ceiling gates.
- Designed and deployed an interactive Human-in-the-Loop (HITL) curation gate using native DuckDB file loops to automatically capture and filter out demographic fairness gaps, severe clinical outliers, and physical hardware sensor dropouts.


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
