# 💼 IBM Data Engineering Capstone Project

[![GitHub](https://img.shields.io/badge/Capstone-IBM%20Data%20Engineering-blue)](https://github.com/Andres-GP/IBM-Data-Engineering-Professional-Certificate-Capstone-Project)

This is the **final capstone project** for the **IBM Data Engineering Professional Certificate**, showcasing an **end-to-end data engineering pipeline**.  
It includes **data extraction, transformation, and loading (ETL)**, **data quality checks**, and **pipeline orchestration** with **Airflow**, all deployed on **AWS Cloud Services**.

---

## 🚀 Live Demo / Project Overview

While this project is primarily backend/data engineering, here is an overview of the workflow:

- Extracts data from APIs and relational databases (PostgreSQL/RDS).
- Transforms and cleans datasets using **AWS Glue** (Spark).
- Stores raw and transformed data in **S3 buckets**, organized by ingestion date.
- Validates data quality using **Glue Data Quality rulesets**.
- Orchestrates pipelines with **Airflow DAGs**.
- Prepares final datasets for **analytics, reporting, or DBT modeling**.

---

## ✨ Features

- 🗄 **Data Extraction** from multiple sources:
  - Public APIs (Users, Sessions endpoints)
  - Relational DBs (RDS/PostgreSQL)
- 🔄 **Data Transformation**:
  - Clean and enforce schemas
  - Enrich data with metadata
  - Convert to **columnar Iceberg format** for efficiency
- ✅ **Data Quality Checks** with AWS Glue rulesets
- 📦 **Pipeline Orchestration** with **Apache Airflow DAGs**
- 🛠 **Cloud Infrastructure** with Terraform to provision AWS resources
- 📊 **Ready for analytics** and DBT modeling
- 🚀 **End-to-end automated ETL pipeline**

---

## 🧰 Tech Stack

| Category                   | Technology                         |
| -------------------------- | ---------------------------------- |
| **Pipeline Orchestration** | Apache Airflow                     |
| **ETL / Transformation**   | AWS Glue (Spark), PySpark          |
| **Data Storage**           | AWS S3 (landing & transform zones) |
| **Relational DB**          | PostgreSQL (AWS RDS)               |
| **Infrastructure as Code** | Terraform                          |
| **Data Modeling**          | DBT                                |
| **Programming**            | Python (PySpark, requests, boto3)  |
| **Scheduling**             | Airflow DAGs                       |
| **Data Quality**           | AWS Glue Data Quality Rulesets     |
| **Format & Storage**       | CSV (raw), Iceberg (transformed)   |

---

## ⚙️ CI/CD & Automation

The project includes best practices for automation and reproducibility:

- **Infrastructure as Code (IaC)** with **Terraform**:
  - Automatically provisions S3 buckets, Glue roles/jobs, and RDS connections.
  - Ensures reproducible cloud setup.

- **Pipeline Orchestration (Airflow DAGs)**:
  - Scheduled runs with **catchup & retries**.
  - Modular tasks: extract → transform → data quality → DBT.

- **Data Validation & Monitoring**:
  - Glue Data Quality rulesets validate transformed tables.
  - Alerts configured for failed DAG runs (via Airflow).

- **Versioned Data Storage**:
  - Landing zone for raw data
  - Transform zone for Iceberg-format cleaned data
  - Partitioned by ingestion date for efficient querying

---

💡 **In short:**  
This capstone demonstrates **full proficiency in modern data engineering**: designing ETL pipelines, orchestrating workflows, ensuring data quality, using cloud infrastructure, and preparing datasets for analytics or modeling.
