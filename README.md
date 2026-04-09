# 🚀 AWS Lambda Serverless API

A simple serverless API built using AWS Lambda and API Gateway. This project demonstrates how to create, deploy, and expose a backend service without managing servers.

---

## 📌 Project Overview

This project showcases a basic serverless architecture where:

* AWS Lambda executes backend logic
* API Gateway exposes the Lambda function as an HTTP endpoint
* The API is tested directly from a browser

---

## 🧩 Architecture

Client (Browser) → API Gateway → AWS Lambda → Response

---

## ⚙️ Tech Stack

* AWS Lambda (Python)
* Amazon API Gateway (HTTP API)
* AWS Management Console
* Python 3.x

---

## 🚀 Features

* Serverless backend (no server management)
* REST API exposure using API Gateway
* Automatic scaling with AWS Lambda
* Simple and lightweight implementation

---

## 📸 Screenshots

### 🔹 Step 1: Lambda Function Created

![Lambda Function](screenshots/lambda-function.png)

### 🔹 Step 2: Lambda Code

![Lambda Code](screenshots/lambda-code.png)

### 🔹 Step 3: API Gateway Integration

![API Gateway](screenshots/api-gateway.png)

### 🔹 Step 4: Final Output (Browser)

![Output](screenshots/browser-output.png)

### ⚠️ Step 5: Concurrency Error (Learning)

![Error](screenshots/concurrency-error.png)

---

## 💻 Lambda Function Code

```python
def lambda_handler(event, context):
    return {
        'statusCode': 200,
        'body': 'Hello from Lambda 🚀'
    }
```

---

## 📊 Sample Response

```
{
  "statusCode": 200,
  "body": "Hello from Lambda 🚀"
}
```

---

## 💡 Key Learnings

* AWS Lambda enables serverless execution without infrastructure management
* API Gateway allows exposing Lambda as a REST API
* Lambda automatically scales based on incoming requests
* AWS enforces a minimum unreserved concurrency (100) at account level
* Concurrency controls help manage load and protect downstream systems

---

## ⚠️ Challenges Faced

* Encountered concurrency limit error while setting reserved concurrency
* Learned how AWS manages resource allocation and prevents overuse

---

## 🔮 Future Enhancements

* Integrate with Amazon DynamoDB
* Add authentication (JWT / Cognito)
* Implement logging and monitoring using CloudWatch
* Deploy using Infrastructure as Code (Terraform / AWS SAM)

---

## 📚 References

* AWS Lambda Documentation
* AWS API Gateway Documentation

---

---

## 🙌 Author

Your Name
GitHub: https://github.com/your-username
