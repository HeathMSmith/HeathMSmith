![Banner](./assets/banner.png)

# 👋 Hi, I'm Heath

I design production-grade AWS infrastructure using Terraform, with a focus on private networking, security, and cost-efficient architecture.

Most of my work avoids common shortcuts (like public subnets and NAT Gateways) and instead emphasizes real-world, enterprise-aligned patterns.

---

## 🚀 Featured Project

### 🧱 Production Web Application (AWS + Terraform)

A production-style AWS architecture built to simulate real-world infrastructure patterns:

- Application Load Balancer + Auto Scaling Group
- Private EC2 instances (no public IPs)
- AWS Systems Manager (SSM) for secure access (no SSH)
- VPC Interface Endpoints (no NAT Gateway required)
- HTTPS via ACM + Route 53

👉 **Key Architectural Decision:**
Eliminated NAT Gateway dependency by leveraging VPC Endpoints and private DNS, reducing cost while maintaining full private connectivity.

[View Example](https://github.com/HeathMSmith/terraform-aws-modules-hms/tree/main/examples/production-webapp)

---

## 📊 What This Project Validates

- Load balancing across multiple instances
- CPU-based auto scaling behavior
- Secure instance access via SSM in a private VPC
- End-to-end HTTPS configuration with ACM + Route 53
- Fully private architecture with zero public compute exposure

---

## 🧠 Core Focus Areas

- Designing private, production-grade AWS VPC architectures
- Infrastructure as Code using Terraform (modular and reusable)
- Secure access patterns (SSM, no SSH, least privilege IAM)
- Cost-efficient architecture (eliminating unnecessary managed services)

---

## 📁 Repository Structure

- `modules/` → reusable Terraform modules  
- `examples/` → real-world implementations  
- `environments/` → (planned expansion for multi-env deployments)

---

## 🔗 Explore the Project

👉 https://github.com/HeathMSmith/Terraform-Master-HMS/tree/main/examples/production-webapp

Includes:
- Terraform modules and example implementation
- Production-style architecture patterns
- Validation of scaling, networking, and secure access

---

## 📫 Connect

- LinkedIn: https://www.linkedin.com/in/heath-m-smith/