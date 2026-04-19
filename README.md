# Superstore Data Analysis – AWS Data Engineering Project

## Overview
This project demonstrates an end-to-end data engineering pipeline on AWS using the Superstore dataset. The goal is to transform raw sales data into meaningful business insights using a serverless architecture.

The pipeline covers the complete lifecycle: data ingestion, transformation, querying, and visualization.

## Problem Statement
Retail businesses generate large volumes of sales data, but analyzing raw CSV files is inefficient due to slow processing and lack of scalability. 

This project solves that problem by building a cloud-based data pipeline that converts raw data into optimized, analytics-ready format and enables fast querying and visualization.

## Architecture
Raw CSV → Amazon S3 → AWS Glue Crawler → AWS Glue (ETL) → Parquet (S3) → Amazon Athena → Amazon QuickSight

## Tech Stack
- Amazon S3 – Data storage (Data Lake)
- AWS Glue – ETL processing
- AWS Glue Crawler – Schema detection and cataloging
- Amazon Athena – SQL-based querying
- Amazon QuickSight – Data visualization
- AWS IAM – Security and access control

## Workflow

1. Data Ingestion
- Uploaded Superstore CSV dataset to Amazon S3

2. Data Cataloging
- Used Glue Crawler to automatically detect schema
- Created tables in Glue Data Catalog

3. Data Transformation (ETL)
- Cleaned and transformed data using AWS Glue (PySpark)
- Converted CSV to Parquet format
- Partitioned data by year and month

4. Data Querying
- Queried processed data using Amazon Athena
- Performed analysis like sales trends, profit, and top products

5. Data Visualization
- Built dashboards in Amazon QuickSight
- Visualized KPIs such as Total Sales, Profit Trends, and Regional Performance

## Key Insights
- Identified top-performing products
- Analyzed monthly sales trends
- Found region-wise profit distribution
- Detected loss-making products

## Key Features
- Fully serverless architecture
- Cost-efficient (pay-per-use services)
- Scalable for large datasets
- Optimized querying using Parquet and partitioning

## What I Learned
- Building real-world data pipelines on AWS
- Writing ETL jobs using PySpark in Glue
- Optimizing data using partitioning and columnar formats
- Querying large datasets efficiently using Athena
- Creating business dashboards with QuickSight

## Future Scope
- Add real-time streaming using AWS Kinesis
- Implement machine learning models for sales prediction
- Automate pipeline using Airflow or Step Functions        

## Screenshots
(Add your QuickSight dashboard screenshots here)

## How to Run
1. Upload dataset to S3
2. Run Glue Crawler
3. Execute Glue ETL job
4. Query using Athena
5. Visualize in QuickSight
