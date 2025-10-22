# 🚀 Databricks ETL Project — Medallion Architecture | Unity Catalog | Delta Lake | BI Dashboard

> **Beginner-to-Intermediate End-to-End Data Engineering Project**  
> 🧠 *Azure Databricks | PySpark | SQL | Delta Optimization | BI Dashboard*

This project demonstrates how I built a **complete ETL pipeline** on Databricks — starting from raw data ingestion to delivering interactive business insights through BI dashboards.  
The implementation leverages **Medallion Architecture**, **Unity Catalog** for governance, **Delta Lake** for reliability and performance, and **Databricks BI Dashboard** for visualization.

📺 **Reference Tutorial:** [Watch the full walkthrough](https://youtu.be/hUTDVTuZO60?si=yoJuF7wgkG3BTLUv)

---

## 🪄 Project Highlights

- 📥 Built a scalable **ETL pipeline** using **Medallion Architecture** (Bronze → Silver → Gold)  
- 🧭 Implemented **Unity Catalog** for governance, security, and data lineage  
- ⚡ Leveraged **Delta Lake features**: Time Travel, Cloning, Vacuum, Table Utilities  
- 🧰 Used both traditional and modern **Delta optimization techniques**  
- 🧾 Applied **Table Utility Commands** to manage tables effectively  
- 📊 Designed a **Databricks BI Dashboard** to visualize KPIs and trends  
- 🔐 Implemented **Row-Level & Column-Level Security** for controlled data access

---

## 🧭 Architecture Overview

![Medallion Architecture Diagram](./assets/medallion_architecture_diagram.png)

1. **Data Ingestion (Bronze)** — Raw Superstore dataset ingested from ADLS Gen2  
2. **Data Cleaning (Silver)** — Data validation, deduplication & formatting  
3. **Data Transformation (Gold)** — Business rules, aggregations, hierarchies & KPIs  
4. **Visualization** — Dashboard creation directly in Databricks

---

## 🧰 Tech Stack

| Category                  | Tools / Tech Used                                |
|---------------------------|--------------------------------------------------|
| Data Platform             | Azure Databricks                                 |
| Storage                   | ADLS Gen2, Delta Tables                           |
| Governance                | Unity Catalog                                    |
| Language                  | PySpark, SQL                                     |
| Architecture              | Medallion (Bronze, Silver, Gold)                  |
| Optimization              | Delta Optimization Techniques                     |
| Visualization             | Databricks BI Dashboard                           |

---

## 🧱 Unity Catalog — Object Model

- ✅ Create Metastore  
- ✅ Create Credential  
- ✅ Create External Locations  
- ✅ Create Catalog & Schema  
- ✅ Create Delta Tables  
- 🔐 Implement RLS/CLS for access control

---

## 🧠 Delta Lake Features Implemented

- Managed vs External Delta Tables  
- DML Commands (Insert, Update, Delete)  
- Vacuum with Dry Run  
- Version History & Time Travel  
- Deep vs Shallow Clone  
- Table Utility Commands  
- Checkpoints & Optimization Techniques

---

## 🧰 Table Utility Commands Used

- `DESCRIBE TABLE` / `DESCRIBE DETAIL` / `DESCRIBE HISTORY`  
- `OPTIMIZE` / `ZORDER BY`  
- `ALTER TABLE ... SET TBLPROPERTIES`  
- `ALTER TABLE ... SET TAGS`  
- `SHOW TBLPROPERTIES`  
- `RESTORE TABLE TO VERSION AS OF`  
- `DROP TABLE`, `VACUUM`, `CHECKPOINTS`

---

## ⚡ Optimization Techniques

### Traditional
- OPTIMIZE Command  
- ZORDER BY  
- Auto Optimize & Auto Compact  
- Caching  
- Data Skipping  
- Partitioning

### Modern
- Liquid Clustering  
- Deletion Vectors  
- Change Data Feed (CDC)  
- Schema Evolution

---

## 📊 BI Dashboard

![Dashboard Screenshot](./assets/dashboard_screenshot.png)

### Key Metrics:
- **Total Sales:** $1.81M  
- **Total Profit:** $437.37K  
- **Total Quantity Sold:** 29.96K  

### Dashboard Features:
- 📈 Year-over-Year Sales vs Profit Trend  
- 🛍️ Category-wise distribution  
- 🌍 Region-level filter  
- 🔄 Real-time insights inside Databricks

---

## 📓 Project Notebooks

| Notebook | File | Description |
|----------|------|-------------|
| 01 | `01_data_ingestion_bronze.ipynb` | Ingest raw data into Bronze layer |
| 02 | `02_data_cleaning_silver.ipynb` | Data cleaning, validation, transformation |
| 03 | `03_data_transformation_gold.ipynb` | Business logic, aggregation, KPI creation |
| 04 | `04_hierarchy_creation.ipynb` | Hierarchy & dimensional modeling |

All notebooks are included in the [`notebooks/`](./notebooks) directory for reference.

---

## 🛡️ Data Governance & Security

- ✅ Row-Level Security (RLS)  
- ✅ Column-Level Security (CLS)  
- 🪄 Data Lineage through Unity Catalog

---

## 📚 Key Learnings

- Designing and implementing **Medallion Architecture** on Databricks  
- Real-world **Unity Catalog** setup and governance  
- Deep dive into **Delta Lake features**: versioning, cloning, optimization  
- Building ETL pipelines using **PySpark + SQL**  
- Dashboarding inside Databricks for fast insights  
- Applying **data governance** best practices in analytics

---

## 🚀 Future Enhancements

- ⚡ Automate the pipeline using Databricks Workflows  
- 📡 Incremental & streaming ingestion  
- 📊 Integrate with Tableau / Power BI for richer visualizations  
- 🧪 Add data quality checks & monitoring  
- 🛡️ Implement CI/CD with Unity Catalog & GitHub Actions

---

## 👨‍💻 Author

**Rishikesh Gundla**  
📊 Senior BI Engineer | 📍 India  
🔗 [LinkedIn](https://www.linkedin.com/in/rishikeshgundla/)

---

⭐ *If you found this project useful, give it a star to support!*  
📝 *This is part of my data engineering portfolio demonstrating real-world Databricks ETL implementation.*
