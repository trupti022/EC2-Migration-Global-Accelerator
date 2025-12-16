# 🌍 EC2 Migration & Global Accessibility using AWS Global Accelerator

## 📌 Project Overview
This project demonstrates disaster recovery and global accessibility by migrating an EC2 instance
from N. Virginia (us-east-1) to Mumbai (ap-south-1) using an AMI, and routing user traffic
automatically to the nearest AWS region using AWS Global Accelerator.

---

## 🧱 Architecture
- EC2 instance in N. Virginia (us-east-1)
  
- AMI creation and cross-region copy
  
- EC2 instance launched in Mumbai (ap-south-1)
  
- AWS Global Accelerator with multiple regional endpoints

---

## 🛠 Implementation Steps

### 1️⃣ EC2 & AMI Creation (us-east-1)
- Launched an EC2 instance in N. Virginia
  
- Installed Apache web server
  
- Hosted a simple web page displaying: **Welcome from N. Virginia**

---

- Created an AMI from the EC2 instance

---

### 2️⃣ Instance Migration to Mumbai (ap-south-1)
- Copied the AMI from us-east-1 to ap-south-1
  
- Launched a new EC2 instance using the copied AMI
  
- Updated the web page to display: **Welcome from Mumbai**


---

### 3️⃣ AWS Global Accelerator Setup
- Created an AWS Global Accelerator
  
- Configured a listener on port 80
  
- Added two endpoints:
  
  - EC2 instance in N. Virginia
    
  - EC2 instance in Mumbai
    
- Enabled health checks to ensure availability

---

### 4️⃣ Testing & Validation
- Accessed the Global Accelerator DNS endpoint
  
- Verified traffic routing based on geographic location
  
- Confirmed automatic failover and region-based routing

---

## ✅ Outcome
- Successful cross-region EC2 migration using AMI
  
- Low-latency global access using AWS Global Accelerator
  
- Improved availability and disaster recovery capability

---

## 🔧 AWS Services Used
- Amazon EC2
  
- Amazon AMI
  
- AWS Global Accelerator
  
- Apache Web Server

---


