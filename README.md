E-Commerce Big Data Analytics
Overview
E-Commerce – Customer Behaviour and Sales Intelligence. This project analyzes sales, customer trends, product demand, payments and delivery performance using the Brazilian Olist public dataset, Apache Spark, Databricks and Power BI.
Team
K.R. Mangalam University | B.Tech CSE
Devansh Kumar – 2401730127; Abhishek – 2401730058; Rohit Kumar – 2401730106. Individual contributions must be confirmed by the team.
Data source
Brazilian E-Commerce Public Dataset by Olist: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce . Nine related CSV tables: customers, geolocation, order items, payments, reviews, orders, products, sellers and category translation. These are one dataset, not nine independent sources.
Architecture
Public CSV dataset → Databricks raw volume → Bronze (ingestion) → Silver (cleaning and joins) → Gold (analytics) → CSV exports → Power BI local model. Delta Lake is the intended storage format. The saved dashboard uses embedded summary data rather than a live Databricks connection.
Engineering workflow
The prepared notebooks cover ingestion with source metadata, cleaning and transformation, analytical aggregations and validation. Import and run 01_Bronze_Data_Ingestion, 02_Silver_Cleaning, 03_Gold_Analytics and 04_Validation in order. Raw volume path: /Volumes/workspace/ecommerce_bigdata/raw_data/. Verify actual workspace execution and export the executed notebooks.
Results from supplied Gold exports
Monthly revenue totals R$13,494,400.74; monthly order counts sum to 98,199. Delivery summary reports 96,478 delivered orders, 12.5 average delivery days and 8.11% late deliveries. Payment value totals R$16,008,872.12, including R$12,542,084.19 by credit card. São Paulo leads state revenue at R$5,163,867.22. Payment value and item revenue are different metrics; monthly order counts and delivery-status counts (98,207) differ and require reconciliation before claiming a single exact order total.
Dashboard and repository
Open 04_PowerBI_Dashboard/Ecommerce_Analytics_Dashboard.pbix in Power BI Desktop. The report shows four KPI cards and six charts covering monthly revenue, categories, states, monthly customers, payments and delivery status. Repository: https://github.com/DevanshKumar01/Ecommerce-BigData-Analytics
Repository structure
02_Processed_Data: six Gold CSV exports (order-items fact is a 1,000-row preview). 03_Databricks_Notebooks: prepared notebook copies and instructions. 04_PowerBI_Dashboard: saved PBIX. 05_Project_Report and 06_Presentation: documentation. 07_Screenshots: dashboard evidence. Raw CSVs are available from the cited dataset; backups are kept locally.
Validation and limitations
Dashboard opening was confirmed by the user. Actual notebook execution, Silver-layer checks, reconciliation and successful pipeline screenshots must be verified in Databricks. Confirm whether related Olist tables satisfy the course preference for three sources wherever feasible. Publish the dashboard and test reviewer access. Do not claim live connectivity or full fact-table export.
References
Olist dataset (link above); Apache Spark documentation: https://spark.apache.org/docs/latest/ ; Databricks documentation: https://docs.databricks.com/ ; Power BI documentation: https://learn.microsoft.com/power-bi/ .
