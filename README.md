# End-to-End Data Engineering Pipeline
A scalable end-to-end data pipeline built on Microsoft Fabric using Medallion Architecture to transform raw data into business-ready insights.

## Architecture
![Data Architecture](images/olist-architecture.jpg)

* **Bronze**: Raw data ingested via pipeline, then converted to Delta tables with schema enforcement
* **Silver**: Data cleaning, standardization, and transformations
* **Gold**: Business-ready tables using star schema

---

## Pipeline
![Data Pipeline](pipeline/pipeline.png)
Orchestrated using Microsoft Fabric Pipelines:

* Copy Activity → Ingest raw data from ADLS to Lakehouse
* Bronze Notebook → Apply schema and convert data to Delta tables
* Silver Notebook → Clean and transform data
* Gold Notebook → Data modeling (Star Schema)

---

---

## Tech Stack & Processing

| Category | Technology | Role in Project |
| :--- | :--- | :--- |
| **Processing** | ![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apache-spark&logoColor=white)  | Distributed computing engine used for large-scale transformations across all layers. |
| **Storage Format** | ![Delta Lake](https://img.shields.io/badge/Delta_Lake-00ADFF?style=flat-square&logo=delta-lake&logoColor=white) | Ensuring **ACID transactions** and **schema enforcement** for reliable data storage. |
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-CC2927?style=flat-square&logo=postgresql&logoColor=white) | Core languages used for complex data manipulation and relational querying. |
| **Data Modeling** | **Star Schema** | Designing **Fact and Dimension** tables optimized for efficient BI reporting and analytics. |

---
---


## Dataset

Olist dataset from Kaggle:
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce


---


