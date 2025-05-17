## # AWS VPC and EC2 Web Server Deployment

## OVERVIEW
This project demonstrates how to build a custom Virtual Private Cloud (VPC) on AWS and deploy a web server using an EC2 instance. The setup includes both public and private subnets, a NAT Gateway, route tables, security groups, and an Internet Gateway. This infrastructure simulates a real-world cloud network for hosting web applications.

## 🛠️ Technologies Used
- AWS EC2
- Amazon VPC
- Public/Private Subnets
- Route Tables
- NAT Gateway
- Internet Gateway
- Security Groups
- Amazon Linux 2023

## Architecture Diagram
![vpc and subnets](https://github.com/user-attachments/assets/af154a67-1c63-4e62-928f-fb687433a318)


## Steps Summary

### ✅ Task 1: Create the VPC and Core Resources
- VPC CIDR: 10.0.0.0/16
- One Public Subnet (10.0.0.0/24)
- One Private Subnet (10.0.1.0/24)
- NAT Gateway and Internet Gateway

### ✅ Task 2: Create Additional Subnets
- Public Subnet 2: 10.0.2.0/24
- Private Subnet 2: 10.0.3.0/24
- Updated route tables for both

### ✅ Task 3: Create a Security Group
- HTTP access is enabled from anywhere (port 80)

### ✅ Task 4: Launch a Web Server EC2 Instance
- Amazon Linux 2023 AMI
- Installed Apache, PHP, MariaDB
- Public IP assigned with HTTP access
- Launched web app with startup script

---
## What I Learned
- The role and differences between **Internet Gateway** and **NAT Gateway**
- How **subnets** and **route tables** direct traffic in AWS
- Using **User Data scripts** to automatically configure instances
- Importance of **security groups** in controlling traffic to EC2 instances
- High availability using multiple **Availability Zones**

## 🌐 Public IP Access Result

> *(Insert your screenshot below)*  
![Web App Running](screenshots/ec2-web-page.png)

