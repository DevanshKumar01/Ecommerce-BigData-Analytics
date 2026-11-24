# E-Commerce Big Data Analytics

## Overview
Analysis of the Brazilian Olist e-commerce dataset using Databricks, a Bronze/Silver/Gold pipeline and Power BI.

## How to open
Extract the ZIP fully. Open `04_PowerBI_Dashboard/Ecommerce_Analytics_Dashboard.pbix` in Power BI Desktop. The saved report contains a local DataModel; the fixed project source in `08_Backup/Fixed_PowerBI_Source` uses embedded summary data, not a live Databricks connection. The PBIX was saved and displayed on the user's computer; reopen the extracted copy to verify.

## Folder guide
- 01_Raw_Dataset: nine original CSV files.
- 02_Processed_Data: six Gold exports. The order-items fact export is a 1,000-row preview, not the full fact table.
- 03_Databricks_Notebooks: previously prepared notebook copies and run instructions; compare with actual executed workspace notebooks before submission.
- 04_PowerBI_Dashboard: final user-saved PBIX, preserved unchanged.
- 05_Project_Report and 06_Presentation: previously prepared drafts, not verified final submissions.
- 07_Screenshots: saved dashboard evidence.
- 08_Backup: original project sources, fixed source, original dataset archive and extra query export. The older PBIP may contain the original measure-name conflict; use the final PBIX instead.

## Dashboard
Revenue, order count, delivery days, late delivery percentage, monthly revenue and customer trends, category and state revenue, payment mix and delivery status. Currency: BRL.

## Before submission
- Reopen the PBIX after extraction.
- Export actual executed Databricks notebooks and verify Silver layer and validation results.
- Review and finalize report and presentation drafts against university requirements.
- Keep the backup folder separately if submission size is restricted.
