# 🚀 Full Stack AWS Deployment with Load Balancer

## Objective
Deploy a simple React + Node.js app to AWS EC2 with an Application Load Balancer (ALB) for scalability.

## Architecture
- Frontend (React) on one EC2 instance
- Backend (Node.js) on multiple EC2 instances
- ALB distributes traffic between backend instances

## Setup Steps

### 1️⃣ Launch EC2 Instances
- One for **frontend**
- Two (or more) for **backend**
- Open ports **22 (SSH)** and **80 (HTTP)** in Security Groups.

### 2️⃣ Deploy Backend
```bash
sudo apt update
sudo apt install -y nodejs npm git
git clone https://github.com/YOUR-USERNAME/fullstack-aws-deploy.git
cd fullstack-aws-deploy/backend
npm install
node server.js

