AWS Systems Manager Session Manager — Replacing SSH
Secure, Centralized, and Auditable Access to AWS EC2 Instances
This project demonstrates how AWS Systems Manager Session Manager can be used as an alternative to traditional SSH access for managing Amazon EC2 instances.
The project compares traditional SSH access through TCP port 22 with Session Manager access and demonstrates how an EC2 instance can remain accessible through Session Manager even after inbound SSH access is removed.
————
📌 Problem Statement
Traditional SSH-based access to EC2 instances generally requires:
- Inbound SSH access through port 22
- SSH key-pair management
- Management of access for multiple users
- Additional infrastructure such as bastion hosts in some architectures
- Additional effort for centralized monitoring and auditing
As the number of servers and developers increases, managing SSH access can become more difficult.
————
🎯 Project Objective
The objective of this project is to demonstrate a more centralized approach to EC2 remote administration using:
- AWS Systems Manager Session Manager
- IAM-based authorization
- SSM Agent
- Amazon CloudWatch Logs
- Amazon S3
The implementation demonstrates that an EC2 instance can be accessed through Session Manager without requiring inbound SSH port 22.
————
🏗️ Architecture
Traditional SSH Architecture
Developer
    |
    | SSH
    | TCP Port 22
    ↓
Security Group
    |
    ↓
EC2 Instance