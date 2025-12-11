# AWS EC2 Docker NGINX CI/CD 🚀

## Project Overview
This project shows a simple DevOps pipeline using:
- Docker
- NGINX
- GitHub Actions CI/CD
- AWS EC2

Whenever code is pushed to GitHub, the new version is automatically deployed to an EC2 instance.

---

## Tech Stack
- Docker
- NGINX
- GitHub Actions
- AWS EC2
- Docker Compose

---

## Architecture Flow
Developer → GitHub → GitHub Actions → Build Docker Image → SSH to EC2 → Run Container → NGINX → Browser

---

## Project Structure
- Dockerfile  
- docker-compose.yml  
- src/index.html  
- .github/workflows/cicd.yml  

---

## Run Locally

### Build Image
docker build -t myapp .

### Run Container
docker run -p 80:80 myapp

### Using Docker Compose
docker compose up -d

---

## CI/CD Pipeline
When you push to the **main** branch:
1. GitHub Actions runs automatically  
2. Builds Docker image  
3. Connects to EC2  
4. Deploys the updated container  
5. Website updates instantly  

---

## What I Learned
- Docker basics  
- CI/CD pipeline setup  
- EC2 deployment  
- Docker Compose usage  

---

## Future Improvements
- Add Terraform  
- Use AWS ECR  
- Add monitoring  
