# ec2-static-site-demo

# 🌐 Static Website Hosted on AWS EC2 (Apache)

This project demonstrates how to deploy a static HTML/CSS website on an AWS EC2 instance using Apache. A free responsive template was transferred from the local machine using `scp`.

---

## 🚀 Project Overview

- Launch an EC2 instance (Amazon Linux 2)
- Install and configure Apache Web Server
- Transfer a free HTML/CSS template from local machine using `scp`
- Serve the website via Apache on port 80

---

## 📸 Live Demo

👉 http://<your-ec2-public-ip>

> Replace with your actual EC2 IP if it's publicly accessible.

---

## 🛠️ Technologies Used

- **AWS EC2 (Amazon Linux 2)**
- **Apache HTTP Server**
- **SCP (Secure Copy)**
- **Free HTML Template**

---

## 🧾 Setup Instructions

### 1. Launch EC2 Instance

- AMI: Amazon Linux 2
- Instance type: `t2.micro` (Free Tier)
- Open ports **22 (SSH)** and **80 (HTTP)** in the Security Group

---

### 2. Connect to EC2 via SSH
```bash
ssh -i your-key.pem ec2-user@<your-ec2-public-ip>



### 3. Install Apache
Copy code
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd


### 4. On Your Local Machine: Prepare Template
Download a free HTML/CSS template (e.g., from HTML5 UP, Free CSS)


