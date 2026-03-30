# Cloud Engineering Assessment Platform

A cloud-based technical assessment web application built using AWS services.
This project allows users to attempt a quiz, calculate scores instantly, and store results in a serverless backend.

---

## Project Overview

The **Cloud Engineering Assessment Platform** is designed to evaluate knowledge in:

* Cloud Computing
* AWS Services
* DevOps Fundamentals
* Linux Administration
* Networking
* Automation Concepts

Users can take the assessment through a web interface, and their results are processed and stored using AWS services.

---

## Features

* Interactive technical quiz
* Real-time score calculation
* Timer-based assessment
* Professional result page
* Serverless backend integration
* Result storage in DynamoDB
* Hosted frontend using EC2 and Nginx

---

## Tech Stack

### Frontend

* HTML
* CSS
* JavaScript

### AWS Services Used

* Amazon EC2
* Nginx
* AWS Lambda
* Amazon API Gateway
* Amazon DynamoDB

---

## Architecture

User Browser → EC2 (Nginx) → API Gateway → Lambda → DynamoDB

---

## How It Works

1. User opens the quiz application hosted on EC2.
2. User enters details and attempts the assessment.
3. Frontend sends quiz results to API Gateway.
4. API Gateway invokes AWS Lambda.
5. Lambda processes the request and stores data in DynamoDB.
6. Final score is displayed to the user.

---

## Project Structure

```text
project/
│── index.html
│── README.md
```

---

## Deployment Steps

### 1. Launch EC2 Instance

* Launch a Linux EC2 instance on AWS
* Install and configure Nginx
* Host the frontend quiz application

### 2. Create DynamoDB Table

* Create a table to store quiz results
* Example table name: `QuizResults`

### 3. Create AWS Lambda Function

* Write Python code to receive quiz submission
* Save user data and score to DynamoDB

### 4. Create API Gateway

* Create a POST method
* Connect it to the Lambda function
* Enable CORS

### 5. Connect Frontend to API

* Use JavaScript `fetch()` method
* Send data from `index.html` to API Gateway

---

## Sample Use Case

This project can be used for:

* Technical screening
* Internal employee skill assessment
* Student cloud knowledge evaluation
* Practice project for AWS / DevOps learners

---

## Future Improvements

* Add login system
* Add admin dashboard
* Add leaderboard
* Export results to PDF
* Add analytics and charts

---

## Live Demo



```text
http://quizstack33.duckdns.org/
```

---

## GitHub Repository

https://github.com/hishamc33-max/quizstack

---

## Author

**Hisham C**
Aspiring DevOps & Cloud Engineer

---

## License

This project is created for learning and portfolio purposes.
