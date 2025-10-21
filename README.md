# 🚀 HNG13 DevOps – Stage 0

### 👩‍💻 Author
**Name:** Oluwayemisi Okunrounmu  
**Slack Username:** @Yemisi  
**Email:** [yemmmyc@hotmail.com](mailto:yemmmyc@hotmail.com)  
**GitHub:** [Yemmmyc](https://github.com/Yemmmyc)

---

## 🌍 Live Deployment
**Server IP:** [http://54.221.73.15/](http://54.221.73.15/)  
**Platform:** AWS EC2 (Ubuntu 22.04 LTS)  
**Deployed On:** October 21, 2025  

> Successfully deployed using NGINX web server running on port **80**.

---

## 🧩 Project Overview
This project was completed as part of **HNG13 DevOps Stage 0**.  
The goal was to deploy a live web server that hosts a custom webpage accessible from the internet.

### Objectives
- ✅ Set up and manage a GitHub workflow  
- ✅ Deploy and configure a live NGINX web server  
- ✅ Serve a custom webpage on port 80  
- ✅ Document, test, and automate the deployment process  

---

## 🛠️ Technologies Used
| Tool | Purpose |
|------|----------|
| **NGINX** | Web server |
| **Docker** | Containerization |
| **Bash** | Automation scripting |
| **AWS EC2 (Ubuntu 22.04)** | Cloud hosting |
| **Git & GitHub** | Version control |

---

## 📜 Deployment Script – `deploy.sh`
This script automates the full deployment lifecycle:

- Clones the GitHub repository  
- Builds and runs the Docker container  
- Configures NGINX as a reverse proxy  
- Handles SSH authentication  
- Supports optional cleanup and error handling  

Run the script:
```bash
./deploy.sh
With cleanup option:

bash
Copy code
./deploy.sh --cleanup
🧾 Logs
All deployment logs are saved in:

deploy.log (latest run)

deploy_YYYYMMDD_HHMMSS.log (timestamped)

These logs assist in auditing and troubleshooting deployments.

⚠️ Troubleshooting Guide
Issue	Possible Fix
Port 80 already in use	Stop conflicting service → sudo fuser -k 80/tcp
NGINX not serving custom page	Verify file exists: /var/www/html/index.html
Docker/NGINX permission errors	Run script with sudo
Repository changes not reflecting	Commit and push updates again

🧹 Optional Cleanup
You can clean up all containers and images automatically:

bash
Copy code
./deploy.sh --cleanup
This ensures a clean, idempotent environment for re-deployment.

🧑‍🏫 Author’s Note
This project demonstrates key DevOps principles:

Automation – One-click deployment using deploy.sh

Reproducibility – Consistent results across environments

Documentation – Clear README and structured logs

📨 Contact
📧 Email: yemmmyc@hotmail.com
🌐 GitHub: Yemmmyc
🧠 Project Repository: HNG13 Stage 0 DevOps
