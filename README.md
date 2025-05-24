# Azure Data Engineering End-to-End Project

## Overview

This project demonstrates a real-world data pipeline built entirely using Azure tools:

- **Data Ingestion**: Azure Data Factory
- **Storage**: Azure Data Lake Gen2
- **Transformation**: Azure Databricks (PySpark)
- **Serving**: Azure Synapse Analytics
- **Visualization**: Power BI

---

## Architecture Diagram

![architecture](./architecture-diagram.png)

---

## Services Used

| Service              | Purpose                         |
|----------------------|---------------------------------|
| Azure Data Factory   | Ingest data from external source |
| Azure Data Lake Gen2 | Store raw, transformed data     |
| Azure Databricks     | Transform with PySpark          |
| Azure Synapse        | Query and serve                 |
| Power BI             | Visualize data                  |

---

## Data Flow

1. Data from HTTP API ingested to **bronze layer** (ADF)
2. Cleaned/enriched in Databricks and saved to **silver**
3. Aggregated and loaded into **gold layer**
4. Registered in Synapse for querying
5. Visualized in Power BI

---

## Hands-on Work Included

- Created & triggered ADF pipelines
- Designed lake layers (`bronze/silver/gold`)
- Wrote PySpark transformations in notebooks
- Configured Synapse workspace and ran SQL
- Connected Power BI to Synapse for live reports

---

## Screenshots

| ADF Pipeline | Data Lake | Databricks | Synapse |
|--------------|-----------|------------|---------|
| ![ADF](./assets/adf-pipeline.png) | ![DL](./assets/lake.png) | ![DB](./assets/databricks.png) | ![Synapse](./assets/synapse.png) |

---

## Skills Demonstrated

- Azure resource provisioning
- Cloud-scale ETL/ELT using PySpark
- Data lake architecture (Bronze/Silver/Gold)
- Azure RBAC & Key-based access
- Data reporting using Power BI
