# Static Website CI/CD Deployment Project

## 📌 Overview
This project demonstrates automated deployment of a static website using:

- **Docker** (Nginx container)
- **GitHub Actions** (CI/CD automation)
- **Ubuntu Server**
- **Tailscale** (Private access VPN)
- **SSH Key-based Deployment**

Changes pushed to GitHub trigger CI/CD pipeline → code is securely deployed → Docker container updates the website.

---

## 🏗️ Architecture

Developer → GitHub Repo → GitHub Actions → Ubuntu Server (Tailscale) → Docker (Nginx) → Static Website


---

## 🚀 Features
- Fully automated deployment
- Private cloud setup (via Tailscale)
- Docker container hosting
- Secure SSH transfer
- Zero-downtime app refresh

---

## ⚙️ Tech Stack
| Component | Tech |
|---|---|
Hosting | Ubuntu 22.04  
Reverse Proxy / Web Server | Nginx  
Container Engine | Docker  
CI/CD | GitHub Actions  
VPN | Tailscale  
Language | HTML / Bash  

---

## 🛠️ Commands Used

### Docker Build & Run
```bash
docker build -t mysite .
docker run -d -p 9090:80 --name mysite mysite
