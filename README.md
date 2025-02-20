# Stock Market Kafka Real Time Data Engineering Project

## Introduction 
This project demonstrates a real-time data pipeline to ingest stock market data using Apache Kafka, store the data in Amazon S3, and query it with AWS Athena after cataloging it with AWS Glue.The goal is to efficiently process and analyze stock market data through a well-defined workflow.



## Architecture 
<img src="Architecture.jpg">


## Technologies Used

- **Programming Language:** Python, SQL

- **Amazon Web Services (AWS):**
  - S3 (Simple Storage Service)
  - Athena
  - AWS Glue
    - Glue Crawler
    - Glue Catalog
  - Amazon EC2

- **Confluent Kafka**


## Workflow Overview 📊

1. **Read data from CSV:**
   - Utilize Python to read stock market data from a CSV file, preparing it for further processing.

2. **Send it to Confluent Kafka with Avro schema:**
   - Leverage Confluent Kafka to efficiently stream the data with Avro schema for effective serialization.

3. **Consume, transform, and store individually in AWS S3 as JSON:**
   - Develop a consumer to process and transform the data, storing it individually in AWS S3 in JSON format.

4. **Glue Crawler does its magic, creating a data catalog:**
   - Employ AWS Glue Crawler to automatically discover and catalog the data in the S3 bucket, enhancing data management.

5. **Athena steps in, empowering me to query insights seamlessly:**
   - Utilize AWS Athena for effortless querying and gaining valuable insights from the processed data.


## Prerequisites

Before you begin with the setup, make sure you have the following:

- **Programming Language:** Python 3.6 or higher

- **Amazon Web Services (AWS):**
  - An AWS account with the following services configured:
    - [S3]
    - [AWS Glue] set up with Glue Crawler and Glue Catalog
    - [Athena]

- **Confluent Kafka:** (https://www.confluent.io/)




