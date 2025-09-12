# Module 2 – Lesson 6: Scalability and Elasticity with EC2

## Key Concepts

### Scalability
- The ability of a system to **increase or decrease capacity** based on workload.
- Two main types:
  1. **Vertical Scaling (Scaling Up/Down)**  
     - Increase/decrease instance size (e.g., t2.micro → t3.large).  
     - Limited by the maximum size available for that instance type.  
  2. **Horizontal Scaling (Scaling Out/In)**  
     - Add/remove multiple instances to handle changes in demand.  
     - Provides better fault tolerance and flexibility.  

### Elasticity
- The ability to **automatically add or remove resources** as demand changes.  
- Ensures that you only pay for what you use.  
- Elasticity is achieved through services like **Amazon EC2 Auto Scaling**.  

---

## AWS Tools for Scalability and Elasticity

### Amazon EC2 Auto Scaling
- Automatically adds/removes EC2 instances based on demand.  
- Uses **scaling policies** triggered by CloudWatch metrics (e.g., CPU usage, memory).  
- Ensures the right number of instances are running at all times.  

**Benefits:**
- High availability.  
- Cost savings (no overprovisioning).  
- Seamless handling of traffic spikes.  

---

### Elastic Load Balancing (ELB)
- Distributes incoming traffic across multiple EC2 instances.  
- Improves **fault tolerance** and **availability**.  
- Works together with Auto Scaling for fully elastic architectures.  

---

## Real-World Example
- **E-commerce website**:  
  - During normal traffic: runs with 2 EC2 instances.  
  - During Black Friday sale: Auto Scaling increases to 20 instances.  
  - ELB distributes user traffic evenly across all instances.  
  - After the sale: Auto Scaling reduces back to 2 instances → saves money.  

---

## 📝 Exam Tips
- **Scalability** = ability to handle growth.  
- **Vertical scaling** = change instance size.  
- **Horizontal scaling** = add/remove instances.  
- **Elasticity** = automatic scaling in/out based on demand.  
- **Auto Scaling + ELB** = the key AWS tools for elasticity.  
- Remember: elasticity is what makes AWS cost-efficient by adjusting resources dynamically.  
