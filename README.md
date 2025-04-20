# devops-k8s-cicd-pipeline
This project implements a complete CI/CD pipeline using **Jenkins**, **Ansible**, **Docker**, and **Kubernetes**, deployed on **AWS EC2** infrastructure.

## ⚙️ Tech Stack
- Jenkins (CI Server)
- Ansible (Provisioning & Configuration)
- Docker (Containerization)
- Kubernetes (Container Orchestration)
- AWS EC2 (Deployment Environment)

## 📍 Phases

## Phase 1: Jenkins Setup
This phase includes the setup of a Jenkins CI server on an Amazon Linux 2023 EC2 instance using a t2.micro (free tier) machine. Jenkins was configured to run on port 8080. Java 17 (Amazon Corretto) was installed, and Jenkins was provisioned using the official Jenkins repository.

[Setup Notes & Commands](jenkins/setup-notes.md)
[Jenkins Dashboard Screenshot](jenkins/screenshots/jenkins_dashboard.png)

### Upcoming Phases
- Phase 2: Ansible Playbooks to configure Docker and deploy containers
- Phase 3: Dockerize sample apps and push to Docker Hub
- Phase 4: Deploy containerized apps to Kubernetes cluster (using Minikube/EKS)

## 📸 Screenshots
> Jenkins dashboard, EC2 setup, and Ansible logs will be uploaded as the setup progresses.
