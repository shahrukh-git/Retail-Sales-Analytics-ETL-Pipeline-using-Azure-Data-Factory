# Retail-Sales-Analytics-ETL-Pipeline-using-Azure-Data-Factory

# Project Title: 
* End-to-End Azure Data Factory ETL Pipeline Using Self-Hosted Integration Runtime.
# Tech Stack: 
* Azure Data Factory, Azure Data Lake Gen2, Azure SQL Database, Self-Hosted IR, CSV, Mapping Data Flows

# Summary:
* Designed and implemented an end-to-end ETL pipeline using Azure Data Factory to ingest customer, product, and sales data from local CSV files via a Self-Hosted Integration Runtime (SHIR). 
* The project was executed entirely without Azure Databricks.

# Key Highlights:
* Used Self-Hosted Integration Runtime to securely load CSV files from on-prem/local system into Azure Data Lake Gen2 (Raw zone).
* Applied transformation logic (data cleaning, date formatting, enrichment, hash generation) using ADF Mapping Data Flows.
* Segregated data zones (Raw → Processed) for better pipeline design and data lineage.
* Loaded clean, transformed data into Azure SQL Database for analysis and reporting.

# Outcome:
* Built a cloud-native, production-ready ETL solution using Azure-first technologies and on-premises data connectivity.

# Architecture Overview
Local CSV Files → Self-Hosted IR → Azure Data Lake Gen2 (Raw) → ADF Pipelines & Data Flows → Azure Data Lake Gen2 (Processed) → Azure SQL Database (Reporting)

* Master Pipeline         
<img width="1920" height="1080" alt="Master_Pipeline" src="https://github.com/user-attachments/assets/52becc6d-68e1-4107-8f86-e64920ea7a85" />

* Pipeline for Customers
<img width="1920" height="1080" alt="Pipeline_for_Customers" src="https://github.com/user-attachments/assets/a2d53818-e3a2-4876-924d-b1ac4e516cc9" />

* Data Flow For Customers
<img width="1920" height="1080" alt="Data_Flow_For_Customers" src="https://github.com/user-attachments/assets/5701cbbb-503c-4332-801e-96708f17b4d6" />

* Pipeline for Products
<img width="1920" height="1080" alt="Pipeline_for_Products" src="https://github.com/user-attachments/assets/388405f2-a761-407b-8a1b-c1557338de0b" />

* Data Flow For Prodcts
<img width="1920" height="1080" alt="Data_Flow_For_Prodcts" src="https://github.com/user-attachments/assets/501ae27b-39f6-4d8d-abdf-38de92d57dbf" />

* Pipeline for Sales
<img width="1920" height="1080" alt="Pipeline_for_Sales" src="https://github.com/user-attachments/assets/049fe37f-8c8a-4076-a011-c2e48b03ad8a" />

* Data Flow For Sales
<img width="1920" height="1080" alt="Data_Flow_For_Sales" src="https://github.com/user-attachments/assets/50858fd9-9bf5-47d6-9aec-77bbdc2a5541" />

* Pipeline to load data in sql
<img width="1920" height="1080" alt="Pipeline_to_load_data_in_sql" src="https://github.com/user-attachments/assets/c7bd90cc-3c83-463b-99e8-66bd30691679" />

* Inside of Pipeline
<img width="1920" height="1080" alt="Inside_of_Pipeline" src="https://github.com/user-attachments/assets/be26bff6-64bf-4e9f-aef9-38fde4e58194" />

* Child Pipeline to execute nested loop
<img width="1920" height="1080" alt="Child_Pipeline_to_execute_nested_loop" src="https://github.com/user-attachments/assets/a8fda780-997e-4123-8ffc-824f434c1b17" />




