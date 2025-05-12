# Azure CI/CD-Enabled Data Engineering Pipeline

## Project Overview

This project demonstrates a **modern data engineering pipeline** built on Azure services with a focus on **CI/CD integration** using **Azure DevOps**. It covers incremental data ingestion from Azure Data Lake and GitHub, transformation using **Azure Databricks**, and utilizes **Delta Tables** for scalable and optimized data processing.

---

## End-to-End Workflow

### Step-by-Step Architecture

1. **Data Ingestion**
   - Incremental data is sourced from **Azure Data Lake** and **GitHub repositories**.
   - **Azure Data Factory (ADF)** orchestrates the pipeline to ingest data into the **Bronze Layer**.
   - ADF is also connected to **Azure DevOps** to implement and manage **CI/CD**, ensuring automated deployment of data pipelines.

2. **Data Transformation**
   - Data from the Bronze Layer is transformed using **Azure Databricks**.
   - It is structured, cleaned, and modeled into **fact and dimension tables**.

3. **Data Storage Layers**
   - **Bronze Layer**: Raw data ingested from multiple sources
   - **Silver Layer**: Cleaned and joined data, stored as **Delta Tables**
   - **Gold Layer**: Final curated data for reporting and analysis

---

## Architecture Diagram

![Untitled Diagram](https://github.com/user-attachments/assets/0d66e5ea-3dd0-4271-b98f-107c1b17e492)

---

## Key Concepts Implemented

- **CI/CD Integration with Azure DevOps** for automated deployment of ADF pipelines
- **Delta Lake Format** for scalable, ACID-compliant data transformations
- **Layered Medallion Architecture** (Bronze → Silver → Gold)
- **Databricks Workflows** for orchestrating transformations

---

## Tools & Technologies

- **Azure Data Factory**
- **Azure Databricks**
- **Azure Data Lake**
- **Azure DevOps**
- **Delta Lake**
- **GitHub**

---

## Outcome

This project presents a real-world-ready solution combining **DevOps best practices with data engineering workflows**. With the use of **Delta Lake** and CI/CD automation, it ensures **scalability**, **data accuracy**, and **faster deployment cycles**, making it suitable for enterprise-grade data pipelines.

