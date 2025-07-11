# Global YouTube ETL Pipeline on AWS

## Overview
This project implements a scalable, serverless ETL pipeline to process and analyze global YouTube data using AWS services. It demonstrates how to build an end-to-end data platform using S3, AWS Glue, Lambda, Redshift, and PySpark.

## Architecture
- **Data Source**: YouTube statistics (global)
- **Landing Zone**: Raw files uploaded to Amazon S3
- **ETL Orchestration**:
  - AWS Lambda to trigger ETL
  - PySpark job on AWS Glue for transformation
- **Data Lake Zones**:
  - Raw → Cleansed → Analytics
- **Data Warehouse**: Amazon Redshift for reporting and dashboards

## Components
- `lambda_function.py`: AWS Lambda trigger for ETL orchestration
- `pyspark_code.py`: Glue PySpark job for data transformation
- `s3_cli_command.sh`: CLI commands to interact with S3 buckets

## Folder Structure
```
📁 src/
    ├── lambda_function.py
    ├── pyspark_code.py
    └── s3_cli_command.sh
📁 docs/
    ├── architecture.jpeg
📄 requirements.txt
📄 README.md
```

## Requirements
Make sure to configure your AWS credentials and environment before running.

## Setup
```bash
# Install dependencies
pip install -r requirements.txt
```

## Author
Rahul Kanth Panganamamula
