
 


🚀 Azure ETL Pipeline: Data Extraction, Transformation & Load

📌 Project Overview
This project builds an ETL pipeline using Azure Data Factory (ADF), Databricks, and PySpark** to extract data from SQL Server & GitHub, transform it via Medallion Architecture (Bronze → Silver → Gold), and handle incremental loads using SCD Type 1 (Upsert).  

---

 🏗️ Architecture & Workflow

 🔹 Data Sources
 
- SQL Server – Relational database  
- GitHub – Raw JSON data extraction  

 🔹 Pipeline Workflow
 
1️⃣ Data Ingestion – Extracting data using **Azure Data Factory (ADF)

2️⃣ Staging – Copying raw data into a staging table

3️⃣ Incremental Load Management – Handling changes using SCD Type 1 (Upsert) 

4️⃣ Data Transformation – Processing data in Databricks using PySpark & Delta Lake 

5️⃣ Final Storage – Organizing data into **fact & dimension tables** for analytics  

 🔹Medallion Architecture Implementation 
- Bronze Layer → Raw ingested data  
- Silver Layer → Cleaned & structured data  
- Gold Layer → Aggregated & analytics-ready data  

---

🛠️ Technologies Used  
- Azure Data Factory (ADF) – Data orchestration & pipeline execution  
- Azure Databricks – Data transformation with PySpark  
- Delta Lake & Delta Tables – Optimized storage & performance  
- SQL Server – Structured data storage  

---

 📌 Key Features:
 
✅ Incremental data loads using a watermark column 

✅ SCD Type 1 (Upsert) for efficient data updates

✅ Optimized pipeline execution with parallel processing

✅ Error handling & schema evolution in Delta Tables 

---

 🏆 Challenges & Solutions  

🔹Handling Incremental Loads

✔ Implemented a watermark table to track `last_load_timestamp`  

✔ Ensured SCD Type 1 Upsert** for efficient record updates  

🔹 Parallel Execution Issues

✔ Resolved data conflicts via deduplication strategies in `fact_sales` 

✔ Maintained **consistent schema evolution** in Delta Tables  

