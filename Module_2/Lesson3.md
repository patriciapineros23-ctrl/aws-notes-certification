# Module 2 – Lesson 3: Interacting with AWS & Shared Responsibility Model

## Interacting with AWS Services
All interactions with AWS services are powered by **APIs**.  
There are three main ways to work with AWS:

### 1. AWS Management Console
- Web-based interface  
- User-friendly (point-and-click)  
- Best for beginners or one-time tasks  

### 2. AWS Command Line Interface (AWS CLI)
- Manage multiple AWS services directly from the **command line**  
- Works on **Windows, macOS, and Linux**  
- Enables **automation with scripts**  
- Example: launching EC2 instances with a script  

### 3. AWS Software Development Kits (SDKs)
- SDKs allow you to interact with AWS services **using programming languages**  
- Example: Using the **AWS SDK for Python (boto3)**  
- Best for developers building applications that integrate with AWS  

---

## Shared Responsibility Model

### Customer Responsibilities
- **Security *in* the Cloud**  
  - Customer data  
  - Client-side data encryption  
  - Server-side encryption  
  - Network traffic protection  
  - Platform and application management  
  - OS and network firewall configuration  

### AWS Responsibilities
- **Security *of* the Cloud**  
  - Physical infrastructure (compute, hardware, storage, database, and networking)  
  - Software that runs AWS infrastructure  

---


## 📝 Exam Tips
- **Console** = beginner-friendly, manual tasks  
- **CLI** = automation & scripting  
- **SDKs** = for developers & apps  
- Remember: **Customer is responsible *in* the cloud, AWS is responsible *of* the cloud**  
- Managed services reduce your responsibilities but may cost more  
