
# 🚀 PDFGenZ PlatformOps Lab

> **Production-Inspired DevOps Platform** built using Docker, Kubernetes, Helm, GitHub Actions, ArgoCD, Prometheus, Grafana and AWS EC2 deployment workflow.

![Platform](https://img.shields.io/badge/Platform-DevOps-blue)
![Docker](https://img.shields.io/badge/Docker-Containerization-2496ED)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-326CE5)
![Helm](https://img.shields.io/badge/Helm-Package_Manager-0F1689)
![ArgoCD](https://img.shields.io/badge/GitOps-ArgoCD-EF7B4D)
![Prometheus](https://img.shields.io/badge/Monitoring-Prometheus-E6522C)
![Grafana](https://img.shields.io/badge/Visualization-Grafana-F46800)
![GitHub Actions](https://img.shields.io/badge/CI-GitHub_Actions-2088FF)

---

# 📖 Overview

PDFGenZ PlatformOps Lab is an end-to-end DevOps portfolio project demonstrating how modern applications are built, containerized, deployed, managed, monitored and automated using industry-standard cloud-native technologies.

The project combines CI/CD, GitOps, Kubernetes deployment strategies, monitoring and cloud deployment concepts into a single practical workflow.

---

# 🎯 Objectives

- Build a production-inspired DevOps platform
- Learn Kubernetes deployment lifecycle
- Implement GitHub Actions CI
- Deploy applications using Helm
- Practice GitOps using ArgoCD
- Monitor workloads using Prometheus & Grafana
- Understand deployment automation and rollback

---

# 🏗 Architecture

```text
Developer
    │
    ▼
Git
    │
    ▼
GitHub Repository
    │
    ├──────────────► GitHub Actions (CI)
    │                     │
    │                     ▼
    │              Docker Image Build
    │                     │
    │                     ▼
    │           AWS EC2 Deployment Workflow
    │
    ▼
ArgoCD (GitOps)
    │
    ▼
Kubernetes Cluster (Kind)
    │
    ▼
Helm Release
    │
    ▼
PDFGenZ Application
    │
    ▼
Prometheus
    │
    ▼
Grafana Dashboards
```

---

# 🚀 DevOps Workflow

1. Develop application
2. Commit using Git
3. Push to GitHub
4. GitHub Actions executes CI workflow
5. Docker image is built
6. Helm deploys application
7. Kubernetes runs application
8. ArgoCD synchronizes Git with the cluster
9. Prometheus collects metrics
10. Grafana visualizes infrastructure health

---

# 🛠 Technologies

| Category | Technology |
|-----------|------------|
| OS | Linux (WSL Ubuntu) |
| SCM | Git, GitHub |
| Containerization | Docker |
| Orchestration | Kubernetes (Kind) |
| Package Manager | Helm |
| Cloud | AWS EC2 (Deployment Workflow) |
| CI | GitHub Actions |
| GitOps | ArgoCD |
| Monitoring | Prometheus |
| Dashboards | Grafana |
| Web Server | Nginx |

---

# 📂 Repository Structure

```text
pdfgenz-platformops-lab/
│
├── .github/workflows/
├── app/
├── argocd/
├── helm/
│   └── pdfgenz/
├── k8s/
├── monitoring/
├── logging/
├── security/
├── Dockerfile
├── .gitignore
└── README.md
```

---

# ⚙️ Prerequisites

- Docker Desktop
- WSL Ubuntu
- kubectl
- Kind
- Helm
- Git
- GitHub Account

---

# 🐳 Docker

Build

```bash
docker build -t pdfgenz-platformops-lab .
```

Run

```bash
docker run -p 8080:80 pdfgenz-platformops-lab
```

---

# ☸ Kubernetes

Deploy

```bash
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
```

Verify

```bash
kubectl get pods
kubectl get svc
```

---

# ⚙ Helm

Install

```bash
helm install pdfgenz ./helm/pdfgenz
```

Upgrade

```bash
helm upgrade pdfgenz ./helm/pdfgenz
```

History

```bash
helm history pdfgenz
```

Rollback

```bash
helm rollback pdfgenz <revision>
```

---

# ☁ AWS EC2 Deployment Workflow

The repository contains a GitHub Actions workflow demonstrating deployment to an AWS EC2 instance through SSH.

The EC2 instance is intentionally kept stopped when not in use to reduce AWS Free Tier usage and avoid unnecessary costs.

---

# 🔄 GitHub Actions

Implemented Continuous Integration workflow that:

- Runs on push
- Validates project
- Builds Docker image
- Supports deployment workflow

---

# 🚀 GitOps with ArgoCD

ArgoCD continuously compares the desired state stored in Git with the live Kubernetes cluster.

Features:

- Git as Source of Truth
- Sync Status
- Drift Detection
- Manual Synchronization
- Automated Deployment Workflow

---

# 📊 Monitoring

## Prometheus

Collects:

- CPU Metrics
- Memory Metrics
- Node Metrics
- Pod Metrics
- Resource Utilization

## Grafana

Visualizes:

- CPU Usage
- Memory Usage
- Network Traffic
- Disk Usage
- Node Health

---

# 🔁 Rolling Updates

Helm upgrades demonstrate zero/minimal downtime deployment using Kubernetes rolling updates.

---

# ↩ Helm Rollback

Rollback to a previous stable release:

```bash
helm rollback pdfgenz 3
```

---

# 💡 Skills Demonstrated

- Linux Administration
- Git & GitHub
- Docker
- Kubernetes
- Helm
- GitHub Actions
- CI/CD
- GitOps
- ArgoCD
- Prometheus
- Grafana
- Deployment Automation
- Monitoring & Observability
- Cloud Deployment Concepts

---

# 🔮 Future Enhancements

- Terraform
- AWS EKS
- Horizontal Pod Autoscaler
- Ingress Controller
- Loki / ELK Logging
- Trivy Image Scanning
- SonarQube
- DevSecOps

---

# 👨‍💻 Author

**Syed Arif Ali**

Cloud & DevOps Engineer 

passionate about Cloud Computing, Kubernetes, Platform Engineering, Infrastructure Automation and AI-powered DevOps.

GitHub: https://github.com/Syed-2050                                                                                                                                
Email : Syedarif1907@gmail.com
---

⭐ If you found this repository useful, consider giving it a star.
