# Muralidhar Reddy Anumandla

**Data Engineer | Azure, Databricks, Spark, SQL | Richmond, VA (open to relocation)**

[Portfolio](https://murali-152002.github.io/) · [LinkedIn](https://www.linkedin.com/in/muralidhar-reddy-anumandla-070576241) · [Email](mailto:anumandlamuralidharreddy@gmail.com) · [All projects](https://github.com/Murali-152002/Data-engineering-My-Projects)

Open to Data Engineer roles. I build and support data pipelines on regulated healthcare data, and I like pipelines that are boring to operate: rerunnable, tested, and easy to explain when they fail.

## What I do

Data Engineer on a UnitedHealth Group client engagement since June 2025, with an M.S. in Computer Science from VCU. I work on Azure Data Factory and Databricks pipelines: Kafka-fed ingestion, Delta Lake tables, data quality checks, migrations and production support.

| What | Result |
|---|---|
| Spark job on about 140M rows | Cut from a 20-hour out-of-memory crash to a 2-4 hour run (about 5-10x faster) |
| Production pipelines | Support 25+ pipelines: trace failures to root cause, rerun transient ones, escalate the rest |
| Legacy consent migration | Tested and reconciled about 3.6M records, source against target, before deployment |
| Duplicate records | Fixed a faulty derived column and merge key in an 8-table Kafka-fed pipeline |

## Projects

Built on real public data, with tests and GitHub Actions CI. Everything runs locally, and each README says what is measured and what is not.

**[NYC Mobility Incremental Pipeline](https://github.com/Murali-152002/Data-engineering-My-Projects/tree/main/nyc-mobility-incremental-pipeline)**: 48.7M real NYC taxi trips plus weather. Idempotent monthly Delta MERGE, quarantine table (978,679 bad rows, each with a reason), late-data test that matches a clean load with 0 duplicates, dbt (37 tests), Airflow, CI. A new month loads in about 78 s versus 15.6 min for a full rebuild.

**[CMS Claims Lakehouse](https://github.com/Murali-152002/Data-engineering-My-Projects/tree/main/claims-lakehouse-cms-delta-dbt)**: two real CMS Medicare files (1.56M rows). Bronze/silver/gold on Delta, quarantine and reconciliation checks, idempotent MERGE, dbt (32 tests), CI.

**[Orders Lakehouse + LLM Assistant](https://github.com/Murali-152002/Data-engineering-My-Projects/tree/main/orders-lakehouse-adf-dbt-airflow)** (mock API data): ADF pipeline-as-code with a watermark that only advances on full success, a dbt star schema with 19 tests, Airflow, and a local-LLM assistant that answers pipeline questions through four read-only tools. SQL that tries to write or drop is refused, and tests prove it.

## Tools

| Area | Tools |
|---|---|
| Languages | SQL / T-SQL, Python, PySpark |
| Platform | Azure Databricks, Delta Lake, Unity Catalog, Azure Data Factory, Azure SQL, Kafka, Spark Structured Streaming |
| Modeling and orchestration | dbt, Airflow, dimensional modeling, medallion architecture, incremental loads |
| Engineering | Git and GitHub, GitHub Actions CI, pytest, DuckDB, Ollama (local LLMs), Power BI, Agile/Scrum |

## Right now

- Building: tool-calling LLM assistants with guardrails over pipeline metadata.
- Ask me about: debugging a Spark out-of-memory job, making pipelines safe to rerun, and testing a migration.
