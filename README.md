
# stock-market-kafka-data-engineering-project

## 📚 Table of Contents
- [Architecture](#-architecture)
- [Project Description](#-project-description)
- [Technologies Used](#-technologies-used)
- [Project Workflow](#-project-workflow)
- [How to Run](#-how-to-run)
- [Prerequisites](#-prerequisites)


## ☁️ Architecture 
![Architecture](https://github.com/user-attachments/assets/c49e2b4c-74ae-48b8-9473-7b36c9ddd2df)

## 📈 Project Description
This project demonstrates the flow of stock market data from a CSV file through Apache Kafka into Amazon S3. The ingested data is then processed using AWS Glue Crawler to create tables in the AWS Glue Data Catalog. Finally, AWS Athena is used to run SQL queries and analyze the stock market data efficiently.

## 🔧 Technologies Used
- **Programming Language:** Python
- **Amazon Web Services (AWS):**
  - S3 (Simple Storage Service)
  - Athena
  - Glue Crawler
  - Glue Catalog
  - EC2
- **Streaming Framework:** Apache Kafka

## 🚀 Project Workflow
1. Stock market data (CSV) is streamed through a Kafka producer.
2. Kafka consumer reads the data and uploads it into an S3 bucket.
3. AWS Glue Crawler is triggered to scan and catalog the S3 data into tables.
4. AWS Athena is used to run SQL queries directly on the cataloged tables for data analysis.

## 🛠️ How to Run
- Instructions to start the Kafka server, Zookeeper, Kafka consumer, and producer are provided in the file **`command_kafka.txt`**.
- Ensure you follow the commands step-by-step to successfully start the streaming process.

## 📄 Prerequisites
- Python installed (preferably 3.7 or higher)
- AWS account with access to:
  - S3
  - Glue
  - Athena
  - EC2 instance setup (for Kafka broker)
- Apache Kafka installed on EC2 or locally

## 📅 Built With
- ![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
- ![AWS](https://img.shields.io/badge/AWS-Cloud-orange)
- ![Kafka](https://img.shields.io/badge/Kafka-Streaming-lightgrey)
