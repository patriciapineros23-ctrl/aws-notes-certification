# Module 2 – Lesson 1: Compute in the Cloud

## How are resources provisioned and managed in the cloud?
- Resources in AWS are **provisioned virtually** rather than using physical servers.  
- Virtual servers (EC2 instances) can be **configured, resized, and managed** on-demand.  
- Management includes choosing the **OS**, installing software, connecting over the network, and running commands.

---

## What is the difference between using virtual servers and managing manual servers?
- **Virtual servers (EC2 instances)**  
  - Run on a shared physical host (multi-tenancy).  
  - Managed by AWS hypervisor for **sharing and isolation**.  
  - Can be **vertically scaled** (increase CPU, memory, storage).  
  - Faster provisioning: launch in minutes instead of buying physical hardware.  

- **Manual/physical servers**  
  - Require purchasing and maintaining hardware.  
  - Scaling or upgrading takes longer.  
  - Must handle OS installation, software, and networking manually.

---

## EC2 – Amazon Elastic Compute Cloud
- **Definition:** EC2 is a virtual server in Amazon's cloud, similar to a physical computer but running over the internet.  
- **Key points:**  
  - Instances are virtual machines (VMs) sharing an underlying physical host.  
  - Multi-tenancy: multiple VMs share the same physical hardware, isolated by a hypervisor.  
  - OS options: Windows or Linux.  
  - Software: You choose what runs on the instance.  
  - Vertical scaling: You can resize the instance for more CPU, memory, or storage.

---

## How to request and use an EC2 instance
1. **Choose a virtual machine (VM)**  
   - Select OS (Windows/Linux)  
   - Select software  
   - Select instance type (CPU, memory, performance)  

2. **Connect to the instance**  
   - Linux: SSH  
   - Windows: Remote Desktop Protocol (RDP)  
   - Or use AWS Systems Manager  

3. **Use the instance**  
   - Run commands  
   - Install software  
   - Organize files and resources  
   - Connect with other instances over the network  

---

## What is multi-tenancy in AWS?
- Multiple EC2 instances share the **same physical host machine**.  
- Provides **resource efficiency** while maintaining isolation.  
- Managed by the **hypervisor** which ensures VMs don’t interfere with each other.  
