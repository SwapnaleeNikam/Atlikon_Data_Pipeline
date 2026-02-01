# Atlikon_Data_Pipeline

# FMCG-Data-Engineering
## Overview
This project repository is an **end-to-end Data Engineering pipeline** built using **AWS services**.It demonstrates how to ingest raw data, store it in cloud storage, transform it using ETL processes, and make it available for analysis.The project follows real-world data engineering practices and cloud-based architecture.
## Problem Statement
AtliQon (Parent Company) is a well-established organization with mature OLTP and OLAP systems in place, enabling reliable transactional processing and analytics-driven decision making.AtliQon has recently acquired a rapidly growing nutrition company, Sports Bar (Child Company). Unlike AtliQon, Sports Bar operates only on an OLTP system and lacks a dedicated analytical (OLAP) layer.During the acquisition analysis, several data challenges were identified within Sports Bar’s data ecosystem:
- Data quality issues such as inconsistent and missing values  
- Missing or poorly defined schemas  
- Partial or lost historical data, especially during the company’s hyper-growth phase  
- No centralized analytical model to support reporting and insights
## Architecture  
- Raw transactional data from Sports Bar (OLTP system) is ingested into Amazon S3, It acts as the central data lake
- The project follows the Medallion Archite-cture (Bronze, Silver, Gold) implemented in Databricks
- The Gold-layer denormalized table is consumed by Databricks SQL Dashboards for visual reporting, Databricks Genie for natural language querying and ad-hoc analysis
- <img width="20005" height="11129" alt="project_architecture" src="https://github.com/user-attachments/assets/98f51bc4-8931-48c0-b04a-10a63db7c291" />
## Result & Conclusion
- Successfully ingested raw OLTP data from Sports Bar into Amazon S3, establishing a scalable and durable cloud-based data lake.
- Implemented a Medallion Architecture (Bronze, Silver, Gold) in Databricks, ensuring structured data processing and clear separation of concerns.
- Resolved key data quality issues, including missing values, schema inconsistencies, and duplicate records.
- Standardized and transformed OLTP data into a single denormalized Gold-layer table, optimized for analytics and reporting.
- Enabled self-service analytics through Databricks SQL Dashboards, providing insights into sales, revenue trends, customer behavior, and product performance.
-Integrated Databricks Genie, allowing business users to perform ad-hoc analysis using natural language queries.
