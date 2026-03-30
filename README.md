# 🚀 QuizStack

**QuizStack** is a cloud-based technical assessment platform built and deployed on AWS.  
It allows users to take a timed technical quiz, calculate scores dynamically, and store results in the cloud using a serverless backend.

🌐 **Live Demo:**  
https://quizstack33.duckdns.org

📂 **GitHub Repository:**  
https://github.com/hishamc33-max/quizstack

---

## 📌 Project Overview

QuizStack is designed to simulate a professional technical assessment platform.  
It was developed to gain hands-on experience in **AWS Cloud, Linux, Nginx, Serverless Architecture, API Integration, Database Storage, DNS configuration, and HTTPS security**.

The application consists of:

- A **frontend quiz interface** hosted on **AWS EC2**
- A **serverless backend** built using **AWS Lambda**
- An **API layer** using **Amazon API Gateway**
- A **NoSQL database** using **Amazon DynamoDB**
- A **custom domain** configured with **DuckDNS**
- **HTTPS/SSL encryption** using **Let’s Encrypt + Nginx**

---

## 🛠️ Tech Stack

- **AWS EC2**
- **Nginx**
- **Amazon API Gateway**
- **AWS Lambda**
- **Amazon DynamoDB**
- **DuckDNS**
- **Let’s Encrypt SSL**
- **HTML**
- **CSS**
- **JavaScript**
- **Python (Boto3)**

---

## ✨ Features

- Professional quiz web interface
- Timer-based assessment
- Dynamic score calculation
- Flexible question attempt
- Cloud-based result storage
- Secure live deployment using HTTPS
- Custom domain access
- Real-time API integration

---

## 🏗️ Architecture

### Project Flow

Frontend (HTML/CSS/JS)  
⬇  
Hosted on **AWS EC2 + Nginx**  
⬇  
Sends quiz results to **Amazon API Gateway**  
⬇  
API Gateway triggers **AWS Lambda**  
⬇  
Lambda stores user result into **Amazon DynamoDB**  
⬇  
Accessible through **DuckDNS custom domain + HTTPS/SSL**

---

## 🌐 Live Project

🔗 **Website:**  
https://quizstack33.duckdns.org

---

## 📂 GitHub Repository

🔗 **Repository:**  
https://github.com/hishamc33-max/quizstack

---

## 🔐 HTTPS / SSL Configuration

The application was secured using **Let’s Encrypt SSL certificates** and configured manually in **Nginx**.

### Security Improvements Implemented:
- Enabled **HTTPS**
- Redirected **HTTP → HTTPS**
- Installed SSL certificate using **Certbot**
- Configured **Nginx server blocks** for secure hosting

This ensures encrypted communication for users accessing the live project.

---

## 🚀 Deployment Steps

### 1. Launch AWS EC2 Instance
- Created and launched an EC2 instance
- Connected using SSH

### 2. Install Nginx
- Installed and configured Nginx on the server
- Hosted the frontend quiz application

### 3. Upload Frontend Files
- Uploaded `index.html` and related assets to:
```bash
/usr/share/nginx/html/
```

### 4. Create Backend with AWS Lambda
- Developed a Lambda function using Python
- Used **Boto3** to insert quiz results into DynamoDB

### 5. Configure API Gateway
- Created a POST route (`/submit`)
- Connected it to Lambda
- Enabled **CORS** for frontend communication

### 6. Create DynamoDB Table
- Created a table to store:
  - Name
  - Email
  - Phone
  - Score
  - Attempted Questions

### 7. Connect Frontend to Backend
- Used JavaScript `fetch()` to send quiz results to API Gateway

### 8. Configure Custom Domain
- Mapped EC2 Elastic IP to **DuckDNS**
- Created public access through:
```text
quizstack33.duckdns.org
```

### 9. Enable HTTPS / SSL
- Installed SSL certificate with Let’s Encrypt
- Configured Nginx for secure deployment
- Redirected HTTP traffic to HTTPS

---

## 📸 Screenshots

You can add screenshots here:

- Homepage
- Quiz Questions
- Result Page
- DynamoDB Table
- AWS Console Architecture

Example:

```md
![Homepage](images/homepage.png)
![Results](images/results.png)
![DynamoDB](images/dynamodb.png)
```

---

## 📚 What I Learned

Through this project, I gained hands-on experience in:

- Linux server management
- Nginx web hosting
- AWS EC2 deployment
- API Gateway integration
- Serverless backend development
- DynamoDB data storage
- DNS mapping with DuckDNS
- HTTPS / SSL implementation
- Cloud application deployment workflow

---

## 💼 Resume Project Description

**QuizStack – Cloud-Based Technical Assessment Platform**  
Developed and deployed a live technical assessment web application using **AWS EC2, Nginx, API Gateway, Lambda, DynamoDB, DuckDNS, and HTTPS with SSL**. Implemented serverless result processing, cloud-based storage, custom domain mapping, and secure HTTPS deployment.

---

## 📢 Author

**Hisham C**  
🔗 GitHub: https://github.com/hishamc33-max  
🔗 LinkedIn: *(Add your LinkedIn profile link here)*

---

## ⭐ Conclusion

QuizStack is a complete hands-on cloud deployment project that demonstrates practical understanding of:

- **Cloud Infrastructure**
- **DevOps Basics**
- **Serverless Backend**
- **Linux Hosting**
- **Secure Web Deployment**

---

### If you like this project, feel free to ⭐ star the repository!
