# Azure Retail Sales Analytics Platform

## Project Overview

Designed and implemented an end-to-end Azure Data Engineering solution using Azure Data Lake Storage Gen2, Azure Databricks, PySpark, Delta Lake, Azure Data Factory, and Azure SQL Database.

The project ingests retail sales data, processes it using a Medallion Architecture (Bronze, Silver, Gold), performs incremental loading using Delta Lake MERGE, and loads curated datasets into Azure SQL Database for analytics and reporting.

---

## Architecture

```text
CSV Files
    ↓
ADLS Gen2 Bronze
    ↓
Databricks (PySpark)
    ↓
Silver Delta Tables
    ↓
Databricks Transformations
    ↓
Gold Delta Tables
    ↓
Parquet Export
    ↓
Azure Data Factory
    ↓
Azure SQL Database
```

---

## Technologies Used

- Azure Data Lake Storage Gen2
- Azure Databricks
- PySpark
- Delta Lake
- Azure Data Factory
- Azure SQL Database
- SQL

---

## Key Features

- Bronze, Silver, Gold Medallion Architecture
- Data cleansing and transformation using PySpark
- Delta Lake implementation
- Incremental loading using MERGE operations
- Revenue analytics generation
- ADF-based data movement
- Azure SQL serving layer

---

## Business Outputs

### Customer Revenue

- Revenue by customer
- Revenue by city

### Category Revenue

- Revenue by product category

### City Revenue

- Revenue by city

---

## Project Structure

```text
azure-retail-sales-analytics-platform
│
├── architecture
├── datasets
├── databricks
├── sql
├── screenshots
└── docs
```

---

## Future Enhancements

- Power BI Dashboard Integration
- ADF Scheduling and Triggers
- CI/CD using Azure DevOps
- Monitoring and Alerting