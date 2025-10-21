# 🚀 HNG13 DevOps Stage 0 Project  

[![Built with NGINX](https://img.shields.io/badge/Built%20with-NGINX-brightgreen?logo=nginx)](https://www.nginx.com)
[![Deployed on AWS EC2](https://img.shields.io/badge/Deployed%20on-AWS%20EC2-orange?logo=amazon-aws)](https://aws.amazon.com/ec2/)
[![Made with HTML](https://img.shields.io/badge/Page%20Type-HTML-blue?logo=html5)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Status](https://img.shields.io/badge/Status-Live%20✅-success)](http://54.221.73.15/)

---

## 📂 Project Structure  

hng13-stage0-devops/
├── index.html
└── README.md

yaml
Copy code

---

## 🌍 Overview  

This repository was created as part of **HNG13 DevOps Stage 0**.  
The task demonstrates fundamental DevOps skills — deploying and managing a live NGINX web server that serves a custom HTML page accessible from the internet.

---

## 🧱 Project Details  

| Detail | Description |
|--------|--------------|
| 👩‍💻 **Name** | Oluwayemisi Okunrounmu |
| 💬 **Slack Username** | @yemmmyc |
| ☁️ **Platform** | AWS EC2 (Ubuntu 22.04 LTS) |
| 🌐 **Server URL** | [http://54.221.73.15/](http://54.221.73.15/) |
| 📅 **Deployed On** | October 21, 2025 |

---

## 🧩 Web Page Output  

Welcome to DevOps Stage 0 – Oluwayemisi Okunrounmu (@yemmmyc)
Successfully deployed on AWS EC2
Deployed: October 21, 2025

yaml
Copy code

---

## ⚙️ Deployment Steps  

1. **Update System and Install NGINX**
   ```bash
   sudo apt update && sudo apt install -y nginx
Replace Default NGINX Index Page

bash
Copy code
sudo nano /var/www/html/index.html
Paste in the custom HTML:

html
Copy code
<h1>Welcome to DevOps Stage 0 – Oluwayemisi Okunrounmu (@yemmmyc)</h1>
<p>Successfully deployed on AWS EC2</p>
<p>Deployed: October 21, 2025</p>
Restart NGINX

bash
Copy code
sudo systemctl restart nginx
Verify Deployment
Visit http://54.221.73.15/ in a browser.
You should see your custom message 🎉

🧭 Validation Checklist
✅ Port 80 is open and reachable
✅ NGINX serves the custom index.html
✅ Public IP displays the expected content
✅ Server remains live for grading

🧑‍🏫 Author’s Note
This project demonstrates:

🔧 Hands-on server setup and deployment

⚙️ Configuration management with NGINX

🧠 Clear and professional documentation

📨 Contact
👩‍💻 Name: Oluwayemisi Okunrounmu
💬 Slack: @yemmmyc
📧 Email: yemmmyc@hotmail.com
🌐 GitHub: Yemmmyc
🚀 Live URL: http://54.221.73.15/

✅ Status: Successfully Deployed and Verified on AWS EC2 🎉
