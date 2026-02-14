# ETL Pipeline – PySpark / AWS Glue / Azure ADF

## Project Goal
Simulate a production-style ETL pipeline using Bronze, Silver, and Gold layers to process sales data for analytics.

## Dataset
- Sample Superstore dataset (CSV)  
- Columns include Order Date, Region, Product Category, Sales, Profit, Customer Name, etc.

## Steps / Code Overview
1. **Bronze Layer** – Load raw CSV data and store as Parquet files.  
2. **Silver Layer** – Clean data, handle nulls, convert dates and types.  
3. **Gold Layer** – Aggregate KPIs by region, category, or month.  
4. (Optional) Visualize aggregated KPIs in BI tools (Tableau, Power BI, AWS QuickSight).  

**DAG Diagram (conceptual):**
[Raw CSV Data]
       |
       v
   [Bronze Layer: Raw Parquet]
       |
       v
   [Silver Layer: Cleaned / Transformed]
       |
       v
   [Gold Layer: Aggregated KPIs]
       |
       v
 [BI / Tableau / QuickSight]



## Tools & Technologies
- PySpark  
- Python  
- AWS Glue / Azure Data Factory (simulated locally)  
- Delta Lake / Parquet storage

## Key Learnings
- Designed end-to-end ETL pipeline structure.  
- Learned layered medallion architecture (Bronze/Silver/Gold).  
- Practiced data transformations, validation checks, and aggregations.
