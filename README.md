# 🌐 2-Tier Web Architecture on AWS

---

## 🔒 Project Overview

This project demonstrates a **2-tier web architecture** on AWS, where:
- A **Private EC2 instance** securely hosts a website using Apache2.
- A **Public EC2 instance** serves as a **Reverse Proxy** using Apache2, exposing the website to the internet while protecting backend infrastructure.

This setup follows a secure cloud architecture pattern using custom VPC networking, NAT, and subnet isolation.

---

## ☁️ Technologies Used

- **Amazon VPC**
- **EC2 Instances (Ubuntu)**
- **Public and Private Subnets**
- **Internet Gateway & NAT Gateway**
- **Apache2 Web Server + Reverse Proxy**
- **Route Tables & Security Groups**
- **SSH & MobaXterm**

---

## 📐 Architecture

📁 Architecture Diagram: [`architecture/architecture-diagram.png`](./architecture/architecture-diagram.png.jpg)

**This setup includes:**
- Custom VPC with Public and Private Subnets
- Internet Gateway for Public EC2
- NAT Gateway to allow Private EC2 outbound access
- Public EC2 with Reverse Proxy (Apache)
- Private EC2 hosting the actual web content
- Route Tables & Security Groups configured for access control

---

## 🔧 Setup Steps

The **full deployment instructions** including screenshots and commands are provided in this PDF:

📄 [`deployment-guide.pdf`](./deployment-guide.pdf.pdf)

---

## 📸 Screenshots

📁 [`screenshots/`](./screenshots)

This folder includes visual proof of configuration:

| Screenshot File              | Description                                                |
|-----------------------------|------------------------------------------------------------|
| `vpcs.png`                  | Custom VPC with subnets, NAT Gateway, and IGW setup        |
| `ec2-instances.png`         | EC2 instance dashboard showing public & private instances  |
| `moba-private-ssh.png`      | SSH into private EC2 from public EC2 using private IP      |
| `apache-reverseproxy.png`   | Apache proxy config using `ProxyPass` and `ProxyPassReverse` |
| `final-output.png`          | Website content served from Private EC2 via Public EC2     |

---

## 📝 User Data Scripts

📁 [`user-data/`](./user-data)

Contains the initialization scripts used when launching EC2 instances:

| File Name                   | Purpose                                      |
|----------------------------|----------------------------------------------|
| `public-ec2-userdata.sh`   | Installs Apache & configures Reverse Proxy   |
| `private-ec2-userdata.sh`  | Installs Apache & sets up the webpage        |

---

## ✅ Key Takeaways

- Gained practical hands-on with secure AWS networking
- Understood how to isolate backend servers from the internet
- Learned Apache Reverse Proxy configuration
- Practiced real-world EC2 access flow using SSH and NAT
- Built professional deployment structure using folder hierarchy

---

## 🙋 Author

**Amrutha Varshini**  
B.Tech – Artificial Intelligence & Machine Learning  
Aditya College of Engineering and Technology (2023–2027)  
📍 India

---

