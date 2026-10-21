
an automated ETL pipeline using python ,aws lambda and amazon s3 for csv data cleaning and deduplication
# AWS Lambda Data Cleaning Project

## About the Project
This is a project I made while learning AWS and Python. In this project, I used AWS S3 and Lambda to clean CSV data automatically.

Whenever a CSV file is uploaded to the raw folder in S3, the Lambda function runs automatically. It removes duplicate records, checks missing values, and saves the cleaned file in the processed folder.

## Services Used
- AWS S3
- AWS Lambda
- Python
- CloudWatch

## How It Works
1. Upload a CSV file to the raw folder.
2. S3 triggers the Lambda function.
3. Lambda reads and cleans the data.
4. Duplicate and invalid records are removed.
5. The cleaned file is saved in the processed folder.
6. Logs can be checked in CloudWatch.

## Files
- `lambda_function.py` - Python code for data cleaning.
- `sales_test.csv` - Sample CSV file used for testing.
- `screenshots` - Screenshots of the project.

## What I Learned
While making this project, I learned how to use S3, create a Lambda function, configure an S3 trigger, process CSV files using Python, and check logs in CloudWatch.

This project helped me understand the basic working of an automated ETL process using AWS.

## Author
Student project made for learning AWS and data engineering basics.
