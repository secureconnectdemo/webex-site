🚀 AI Webex Assistant Deployment Guide

This project provides a beautifully styled, self-contained HTML-based deployment guide for Cisco's AI Webex Assistant. It's designed for internal enablement, onboarding, and process optimization.

It includes:

📄 A dark-mode, collapsible HTML guide

🐳 Dockerfile for local or cloud container hosting

🌍 Ready for one-click deployment to Render or any container platform

🔁️ Copy buttons for code snippets

✅ No frameworks or servers required — just pure HTML + NGINX

📂 Folder Structure

webex-site/
├── index.html        # The main guide file (fully styled, interactive)
└── Dockerfile        # Minimal NGINX-based Docker setup

🐳 Run Locally with Docker

Step 1: Build the image

docker build -t webex-docs .

Step 2: Run it

docker run -d -p 8080:80 webex-docs

Step 3: Open in browser

Go to:👉 http://localhost:8080

🌍 Deploy on Render (Free Hosting)

Render is a free platform that runs Docker images with public URLs.

Steps:

Push this repo to GitHub

Go to https://render.com

Click New > Web Service

Choose your GitHub repo

Set environment to Docker

Click Create Web Service

Render will:

Clone your repo

Build and run your Dockerfile

Host your guide at a public HTTPS URL

🐙 Push to DockerHub (Optional)

You can push your container to DockerHub for reuse or collaboration:

docker tag webex-docs yourusername/webex-docs
docker push yourusername/webex-docs

Others can run your bot guide directly with:

docker run -d -p 8080:80 yourusername/webex-docs

🧐 Why Use This?

✅ Share secure onboarding guides without giving dashboard access

✅ Standardize handoffs and CS enablement

✅ Improve adoption with self-service visuals

✅ Scale internal documentation without friction

✍️ Author

Built by [Your Name] — Cisco Customer SuccessLicensed for internal or team use. Contributions welcome!

📬 Feedback

Open an issue or submit a pull request if you have improvements, formatting ideas, or want to contribute.

