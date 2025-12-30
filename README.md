#  End-to-End DevOps CI/CD Project on AWS EKS (GitOps)

## Project Overview
This project demonstrates a complete production-style CI/CD and GitOps workflow using Docker, Kubernetes (AWS EKS), Helm, Jenkins, and Argo CD.

The application consists of:
- Frontend: React served via NGINX
- Backend: Spring Boot REST API
- Database: PostgreSQL (Helm-based)
- Observability DB Integration: Arize Phoenix with PostgreSQL
- Jenkins Pipeline
- ArgoCD for Deployment

## Tech Stack
- Docker
- Kubernetes (AWS EKS)
- Helm
- Jenkins
- Argo CD + Image Updater
- AWS ECR
- React + NGINX
- Spring Boot
- PostgreSQL
- Arize Phoenix


## CI/CD & GitOps Workflow
1. Developer pushes code to GitHub
2. Jenkins pipeline triggers automatically
3. Docker images are built and tagged
4. Images are pushed to AWS ECR
5. Kubernetes manifests / Helm charts updated
6. Argo CD Image Updater detects new image tag
7. Argo CD syncs changes to EKS automatically

## Configuration Management
- ConfigMaps for application configuration
- Kubernetes Secrets for credentials
- Separate configs for backend and Arize Phoenix

# PostgreSQL Deployment Using Helm
## Installation
PostgreSQL is deployed using Helm with:
- PersistentVolumeClaim (AWS EBS)
- Custom username & database
- Kubernetes Secret integration
## Usage
- Backend application
- Arize Phoenix metadata storage

  # Future Improvements
- Prometheus & Grafana
- EventBridge And Lamda
- HPA & Auto Scaling
- Security scanning ( Trivy And OWASP)

  # Architecture


