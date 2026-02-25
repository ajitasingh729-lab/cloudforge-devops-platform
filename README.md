## CloudForge – End-to-End DevOps Platform

## Overview

CloudForge is a full DevOps lifecycle project that demonstrates containerization, CI/CD automation, orchestration, Infrastructure as Code, and configuration management using industry-standard tools.

This project simulates a real-world DevOps workflow from application build to automated deployment.

---

## Tech Stack

- Docker
- GitHub Actions (CI/CD)
- Docker Compose
- Kubernetes (KIND Cluster)
- Terraform
- Ansible
- Flask (Python)
- Nginx (Reverse Proxy)

---

## Architecture Flow

1. Code pushed to GitHub
2. GitHub Actions builds & pushes Docker image to Docker Hub
3. Application deployed using:
   - Docker Compose (multi-container)
   - Kubernetes (Deployment + Service)
4. Infrastructure provisioned using Terraform
5. Deployment automated using Ansible

---

## Docker

Build image:
```bash
docker build -t ajtasingh/cloudforge-app:latest .

## Run container:

docker run -p 5000:5000 ajtasingh/cloudforge-app

## Terraform (Infrastructure as Code)
cd terraform
terraform init
terraform plan
terraform apply
terraform destroy


## Ansible Deployment
cd ansible
ansible-playbook -i inventory.ini deploy.yml

** Author**

Ajita Singh
DevOps | Cloud | Infrastructure Automation


