# Module 2 – Lesson 4: Setting Up an Amazon EC2 Instance

## Key Configurations When Launching an EC2 Instance
When creating an **Amazon EC2 instance**, you need to configure several settings:

1. **Amazon Machine Image (AMI)**
   - A preconfigured template that includes:
     - Operating system (Windows/Linux)  
     - Application server  
     - Applications  
   - Provides a starting point for launching new instances.  

2. **Instance Type**
   - Defines the **hardware capacity**:  
     - CPU, memory, storage, and network performance  
   - Choose based on workload (general-purpose, compute-optimized, memory-optimized, etc.).  

3. **Key Pair (Authentication)**
   - Used to securely connect to your instance.  
   - **SSH keys** for Linux  
   - **RDP (Remote Desktop Protocol)** for Windows  

4. **Networking**
   - Configure the **VPC (Virtual Private Cloud)**, subnets, and security groups.  
   - Security groups act as **firewalls**, controlling inbound and outbound traffic.  

5. **Storage**
   - Define storage volumes using **Amazon EBS (Elastic Block Store)**.  
   - Can attach multiple volumes to an instance.  

---

## Amazon Machine Images (AMIs) and Scaling
- An **AMI** is a blueprint for your instance.  
- AMIs help maintain **consistency and efficiency** by:
  - Allowing you to launch **multiple identical instances** quickly.  
  - Ensuring all instances have the **same OS, configurations, and apps**.  
  - Useful when scaling applications across **Auto Scaling groups**.  

**Example:**  
- You create an AMI of a properly configured web server.  
- When traffic increases, Auto Scaling uses that AMI to launch more servers with the **exact same setup**, ensuring consistency.  

---

## 📝 Exam Tips
- **AMI = template** for launching instances.  
- Remember the **five key configurations**: AMI, instance type, key pair, networking, storage.  
- **Security groups** act like virtual firewalls.  
- AMIs make **scaling consistent and efficient** because every new instance is identical.  

