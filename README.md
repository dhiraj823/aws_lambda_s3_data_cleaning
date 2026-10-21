
an automated ETL pipeline using python ,aws lambda and amazon s3 for csv data cleaning and deduplication
# AWS Lambda S3 Data Cleaning ETL Project

## 📌 Project Description
This project demonstrates a simple serverless ETL (Extract, Transform, Load) data-cleaning pipeline using AWS S3 and AWS Lambda with Python.

When a CSV file is uploaded to the `raw/` folder in an Amazon S3 bucket, an AWS Lambda function is automatically triggered. The function validates and cleans the data, removes duplicate records, and saves the cleaned CSV file to the `processed/` folder.

## 🎯 Project Objectives
- Automate CSV data cleaning.
- Use AWS S3 to store raw and processed data.
- Trigger AWS Lambda automatically when a CSV file is uploaded.
- Validate data and remove duplicate records.
- Monitor execution using Amazon CloudWatch.

## 🛠️ Technologies Used
- AWS S3
- AWS Lambda
- Python
- Boto3
- Amazon CloudWatch
- CSV

## ⚙️ How It Works
1. Upload a CSV file to the `raw/` folder in the S3 bucket.
2. Amazon S3 triggers the Lambda function automatically.
3. The Lambda function reads the uploaded CSV file.
4. It validates required fields and checks numeric values in the amount column.
5. Records with missing or invalid required data are skipped.
6. Duplicate records are removed.
7. The cleaned CSV file is uploaded to the `processed/` folder.
8. Execution details are logged in Amazon CloudWatch.

## 📂 Project Structure
```text
aws-lambda-s3-data-cleaning/
├── lambda_function.py
├── sales_test.csv
├── screenshots/
└── README.md
