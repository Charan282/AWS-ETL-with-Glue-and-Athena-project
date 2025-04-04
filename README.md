# AWS-ETL-with-Glue-and-Athena-project
AWS Data Pipeline: S3, Glue, Athena, and Quicksight

# Project Overview
This project demonstrates an end-to-end data pipeline using AWS services. The pipeline moves data from Amazon S3 to AWS Glue, processes it using PySpark, catalogs it using AWS Glue Crawler, queries it with Amazon Athena, and visualizes it using Amazon Quicksight.

# Workflow
**Setup IAM User & Permissions**: Created a user with necessary policies (Glue, S3, Athena, Quicksight).

**Data Storage in S3**: Uploaded transformed datasets into S3 (staging and datawarehouse folders).

**AWS Glue for ETL:**

1. Extracted, transformed, and loaded data using AWS Glue Jobs.

2. Performed joins and schema optimizations.

3. Converted data into Parquet format for optimized storage and querying.

AWS Glue Crawler:

Created a data catalog to expose S3 datasets as a structured database.

Allowed Athena to query the data efficiently.

Amazon Athena:

Setup Athena query editor to run SQL queries over the structured dataset.

Stored Athena query results in an S3 bucket.

Amazon Quicksight:

Connected to Athena and visualized insights through dashboards.

# Technologies Used
Storage: Amazon S3

ETL & Processing: AWS Glue (PySpark)

Querying: Amazon Athena (SQL)

Visualization: Amazon Quicksight

Access Management: IAM Roles & Policies

# Setup & Execution
Clone this repository:

bash
Copy
Edit
git clone https://github.com/yourusername/AWS-Data-Pipeline.git
cd AWS-Data-Pipeline
Follow the IAM setup instructions to create necessary roles and policies.

Upload sample datasets to an S3 bucket.

Run AWS Glue Job and AWS Glue Crawler.

Execute SQL queries in Athena.

Connect Athena to Quicksight for visualization.

Future Enhancements
Implement AWS Lambda to trigger Glue Jobs on new data arrival.

Automate the entire pipeline using AWS Step Functions.
