# 🚀 AWS EC2 Instance Setup

## 📌 Overview

This project demonstrates the hands-on implementation of launching, configuring, and accessing an Amazon EC2 instance on AWS. It covers the complete workflow from instance creation to secure remote access and basic server interaction.

---

## ☁️ Service Used

- Amazon EC2 (Elastic Compute Cloud)

---

## 🛠️ Implementation Steps

1. **Access AWS Console**
   Navigated to the EC2 Dashboard from the AWS Management Console.

2. **Launch EC2 Instance**
   - Selected **Amazon Linux 2023 AMI**
   - Chose **t2.micro (Free Tier eligible)**
   - Used default configuration settings

3. **Create Key Pair**
   - Generated key pair: `EC2Tutorial.pem`
   - Downloaded securely for SSH access

4. **Configure Security Group**
   - Allowed **SSH (Port 22)**
   - Source: `0.0.0.0/0` _(for learning purposes only)_

5. **Connect to Instance**
   Accessed the instance using SSH:

   ```bash
   ssh -i EC2Tutorial.pem ec2-user@<Public-IP>
   ```

6. **Execute Basic Commands**

   ```bash
   ls
   pwd
   sudo dnf update -y
   ```

---

## 📸 EC2 Setup Workflow

![EC2 Setup](https://raw.githubusercontent.com/snehalnarale05-tech/aws-cloud-practice/refs/heads/main/EC2/screenshots/ec2-instance-setup-workflow.png.png)

---

## ⚠️ Security Note

- The private key (`.pem`) is not included in this repository
- Sensitive information has been removed or masked
- Security group settings are for learning purposes and should be restricted in production

---

## 📚 Learning Outcomes

- Understood EC2 instance lifecycle and configuration
- Learned secure remote access using SSH
- Gained hands-on experience with Linux commands on a cloud server

---

## 🔮 Future Scope

- Deploy a web application on EC2
- Implement Infrastructure as Code (Terraform)
- Configure IAM roles and enhance security practices

---

## 👩‍💻 Author

**Snehal Narale**
B.E. IT Student | AWS & Cloud Learner
