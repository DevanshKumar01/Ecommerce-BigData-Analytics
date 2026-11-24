# Exact Databricks run instructions

1. Catalog > workspace > ecommerce_bigdata > Volumes > Create Volume: `raw_data` (Managed). You already created the schema; create volume only if absent.
2. Open volume > Upload files. Extract `dataset.zip` locally and upload all nine `.csv` files individually. Path should be `/Volumes/workspace/ecommerce_bigdata/raw_data/`.
3. In Databricks Workspace use Import to import `.ipynb` notebooks (or open and copy content if Import unavailable).
4. Run notebooks **in numeric order** 01 Bronze, 02 Silver, 03 Gold, 04 Validation using Serverless compute.
5. If errors occur, capture exact error and notebook cell; do not proceed blindly.
6. Capture screenshots showing successful runs, tables and validation output; note counts and actual date.
7. Export notebooks and create dashboard from Gold tables. Use Power BI or Tableau for the mandatory final visualization.
8. Update report and presentation with verified numbers, real dashboard screenshots and team details before submission.

**Important:** All nine CSVs are tables from one Olist dataset, not independent data sources. Course guidelines say at least three sources wherever feasible; clarify with instructor whether three related tables are accepted or add independent, justified sources.
