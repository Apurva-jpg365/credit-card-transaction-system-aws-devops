# Credit Card Transaction Processing System with Architecture (AWS DevOps)

## 📌 Overview
This project simulates a credit card transaction system with fraud detection using AWS and DevOps practices.

## ⚙️ Features
- Transaction API using Flask
- Fraud detection logic
- Docker containerization
- CI/CD pipeline (AWS CodePipeline)
- Infrastructure as Code (CloudFormation)

## 🛠️ Tech Stack
- Python (Flask)
- AWS (EC2, S3, IAM, CloudWatch, CodePipeline)
- Docker
- Jenkins

## 🚀 How to Run
1. Install dependencies:
   pip install -r requirements.txt

2. Run app:
   python app.py

3. Test API using Postman or curl

## 🧪 Sample API
POST /transaction

{
  "card_number": "1234",
  "amount": 15000
}

## 📊 Output
- Valid Transaction
- Fraud - High Amount

- User / Postman
      ↓
API Gateway
      ↓
EC2 (Docker Flask App) / Lambda
      ↓
Fraud Detection Logic
      ↓
RDS / DynamoDB
      ↓
CloudWatch Logs

CI/CD Flow:
GitHub → CodePipeline → CodeBuild → Deploy

Storage:
S3 (Artifacts + Logs)

Security:
IAM + Security Groups + VPC
