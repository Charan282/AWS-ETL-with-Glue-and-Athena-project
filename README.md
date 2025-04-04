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

**AWS Glue Crawler:**

1. Created a data catalog to expose S3 datasets as a structured database.

2. Allowed Athena to query the data efficiently.

**Amazon Athena:**

1. Setup Athena query editor to run SQL queries over the structured dataset.

2. Stored Athena query results in an S3 bucket.

**Amazon Quicksight:**

Connected to Athena and visualized insights through dashboards.

# Technologies Used
1. **Storage:** Amazon S3

2. **ETL & Processing:** AWS Glue (PySpark)

3. **Querying:** Amazon Athena (SQL)

4. **Visualization:** Amazon Quicksight

5. **Access Management:** IAM Roles & Policies

# Setup & Execution
1. Clone this repository:
```
git clone https://github.com/yourusername/AWS-Data-Pipeline.git
cd AWS-Data-Pipeline
```
2. Follow the IAM setup instructions to create necessary roles and policies.

3. Upload sample datasets to an S3 bucket.

4. Run AWS Glue Job and AWS Glue Crawler.

5. Execute SQL queries in Athena.

6. Connect Athena to Quicksight for visualization.

**Future Enhancements:**
1. Implement AWS Lambda to trigger Glue Jobs on new data arrival.

2. Automate the entire pipeline using AWS Step Functions.
