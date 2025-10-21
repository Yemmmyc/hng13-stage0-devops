🚀 DevOps Stage 1 – Automated Web Server Deployment
🧾 Project Overview

This project automates the deployment of a custom HTML landing page using NGINX and Docker.
It was completed as part of HNG13 DevOps Stage 1, demonstrating end-to-end CI/CD automation on a cloud instance (AWS EC2).

⚙️ Deployment Script Highlights (deploy.sh)

Fully automated end-to-end setup

Supports interactive prompts for user inputs

Automatically handles container rebuilds

Built-in error handling (set -e and trap)

Optional --cleanup flag for idempotent deployments

Logs every deployment action for traceability

🧩 Key Features

✅ Automated cloning and deployment from GitHub
✅ Dynamic timestamped logging for each run
✅ Built-in validation for Docker and NGINX
✅ Health check confirmation before success message
✅ Works on local Linux (WSL) and AWS EC2 Ubuntu

🖥️ How to Run Locally or on a Server

Clone the repository:

git clone https://github.com/Yemmmyc/hng-stage1-devops.git
cd hng-stage1-devops


Make the script executable:

chmod +x deploy.sh


Run deployment interactively:

./deploy.sh


To perform a clean redeploy:

./deploy.sh --cleanup

📂 Logs

All actions are recorded in deploy.log

Timestamped logs (deploy_YYYYMMDD_HHMMSS.log) are created for each run

Useful for debugging and audit tracking

⚠️ Troubleshooting
Issue	Possible Fix
Port 80 already in use	Run sudo fuser -k 80/tcp to free it
NGINX not serving custom page	Verify /var/www/html/index.html exists
Docker/NGINX permission errors	Run the script with sudo
Repository changes not reflecting	Recommit and push updates before redeploy
🧹 Optional Cleanup

Use the cleanup flag to remove all containers and start fresh:

./deploy.sh --cleanup

📦 Deployment Info

Deployed on: AWS EC2 (Ubuntu 22.04 LTS)

Public URL: http://54.221.73.15/

Deployed Date: October 21, 2025

👨‍💻 Author

Name: Oluwayemisi Okunrounmu
Email: yemmmyc@hotmail.com

GitHub: Yemmmyc

🏁 Notes

This project showcases practical DevOps fundamentals:
automation, version control, containerization, and documentation.
