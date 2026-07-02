# aws-devops-node-red-project
# AWS DevOps Project - Node-RED Monitoring Platform

## Overview

This project demonstrates a complete AWS DevOps deployment using Terraform, Docker, Docker Compose, and GitHub Actions.

The infrastructure is provisioned on AWS using Infrastructure as Code (Terraform). The application stack is containerized using Docker and consists of:

* Nginx
* Node-RED
* InfluxDB
* Grafana

The project also includes CI/CD automation using GitHub Actions.

---

# Architecture

```
GitHub Repository
        │
        ▼
GitHub Actions
        │
        ▼
AWS EC2 Instance
        │
        ▼
Docker Compose
│
├── Nginx
├── Node-RED
├── InfluxDB
└── Grafana
```

---

# AWS Services Used

* Amazon EC2
* Amazon VPC
* Public Subnet
* Internet Gateway
* Route Tables
* Security Groups
* Amazon S3
* IAM Roles
* CloudWatch
* Elastic IP

---

# Technologies

* Terraform
* Docker
* Docker Compose
* GitHub Actions
* AWS CLI
* Node-RED
* InfluxDB
* Grafana
* Nginx
* Linux (Ubuntu)

---

# Project Structure

```
aws-devops-node-red-project/

├── .github/
│   └── workflows/
│
├── terraform/
│   ├── modules/
│   ├── provider.tf
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│   └── ...
│
├── docker-compose.yml
├── Dockerfile
├── README.md
└── .gitignore
```

---

# Features

* Infrastructure provisioning using Terraform
* Modular Terraform architecture
* AWS networking setup
* EC2 provisioning
* IAM Role configuration
* Dockerized services
* Automatic deployment using GitHub Actions
* Infrastructure version control
* Remote Terraform state support
* Easy scaling for future services

---

# Infrastructure Created

* VPC
* Public Subnet
* Internet Gateway
* Route Table
* Security Group
* EC2 Instance
* Elastic IP
* S3 Bucket
* IAM Role
* CloudWatch Resources

---

# Application Stack

| Container | Port |
| --------- | ---- |
| Nginx     | 80   |
| Node-RED  | 1880 |
| InfluxDB  | 8086 |
| Grafana   | 3000 |

---

# Prerequisites

* AWS Account
* Terraform
* Docker
* Docker Compose
* Git
* GitHub Account
* AWS CLI

---

# Clone Repository

```bash
git clone https://github.com/<your-github-username>/aws-devops-node-red-project.git

cd aws-devops-node-red-project
```

---

# Configure AWS Credentials

```bash
aws configure
```

---

# Initialize Terraform

```bash
cd terraform

terraform init
```

---

# Validate

```bash
terraform validate
```

---

# Preview Infrastructure

```bash
terraform plan
```

---

# Deploy Infrastructure

```bash
terraform apply
```

---

# Destroy Infrastructure

```bash
terraform destroy
```

---

# Deploy Application

```bash
docker compose up -d
```

---

# Verify Running Containers

```bash
docker ps
```

---

# Access the Applications

Replace `<EC2_PUBLIC_IP>` with your EC2 public IP.

Grafana

```
http://<EC2_PUBLIC_IP>:3000
```

Node-RED

```
http://<EC2_PUBLIC_IP>:1880
```

InfluxDB

```
http://<EC2_PUBLIC_IP>:8086
```

Nginx

```
http://<EC2_PUBLIC_IP>
```

---

# CI/CD Pipeline

The project uses GitHub Actions to:

* Checkout repository
* Authenticate with AWS
* Validate Terraform
* Deploy infrastructure
* Deploy Docker application

---

# Future Improvements

* HTTPS using Let's Encrypt
* Application Load Balancer
* Auto Scaling Group
* ECS Migration
* RDS Integration
* AWS Secrets Manager
* Route 53
* CloudFront
* Prometheus Monitoring
* Kubernetes (EKS)

---

# Screenshots

Add screenshots after deployment.

* AWS Console
* EC2 Instance
* VPC
* Security Groups
* S3 Bucket
* Terraform Apply
* GitHub Actions
* Grafana Dashboard
* Node-RED Dashboard

---

# Learning Outcomes

This project demonstrates practical experience with:

* AWS Infrastructure
* Infrastructure as Code
* Docker Containerization
* CI/CD Automation
* GitHub Actions
* Linux Administration
* Cloud Networking
* Monitoring Solutions
* DevOps Best Practices

---

# Author

**Poornima Devi**

AWS | Terraform | Docker | GitHub Actions | DevOps Engineer

GitHub: https://github.com/<your-github-username>

LinkedIn: https://www.linkedin.com/in/<your-linkedin-profile>
