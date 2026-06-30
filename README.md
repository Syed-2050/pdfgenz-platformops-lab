# 🚀 PDFGenZ PlatformOps Lab

> A production-inspired DevOps project demonstrating containerization, Kubernetes orchestration, GitOps, CI/CD automation, and monitoring using modern cloud-native tools.

---

# 📖 Overview

PDFGenZ PlatformOps Lab is a hands-on DevOps project built to simulate a modern application deployment workflow.

The project demonstrates how an application can be containerized, deployed to Kubernetes, managed with Helm, synchronized using GitOps (ArgoCD), monitored with Prometheus and Grafana, and automated using GitHub Actions.

This project was built to gain practical experience with technologies commonly used by Cloud Engineers, DevOps Engineers, and Platform Engineers.

---

# 🏗 Architecture

```
Developer
    │
    ▼
 GitHub Repository
    │
    ▼
 GitHub Actions (CI)
    │
    ▼
 Docker Image
    │
    ▼
 Kubernetes Cluster (Kind)
    │
 ┌──┴────────────┐
 ▼               ▼
Helm         ArgoCD (GitOps)
 │               │
 └──────┬────────┘
        ▼
 PDFGenZ Application
        │
        ▼
 Prometheus
        │
        ▼
 Grafana Dashboard
```

---

# 🛠 Technologies Used

| Category | Technologies |
|----------|--------------|
| Operating System | Linux (WSL Ubuntu) |
| Version Control | Git, GitHub |
| Containerization | Docker |
| Orchestration | Kubernetes (Kind) |
| Package Management | Helm |
| CI/CD | GitHub Actions |
| GitOps | ArgoCD |
| Monitoring | Prometheus |
| Visualization | Grafana |
| Web Server | Nginx |

---

# 📂 Project Structure

```
pdfgenz-platformops-lab/

├── .github/
│   └── workflows/
│
├── app/
│   └── index.html
│
├── argocd/
│   └── application.yaml
│
├── helm/
│   └── pdfgenz/
│
├── k8s/
│   ├── deployment.yaml
│   └── service.yaml
│
├── monitoring/
│   ├── prometheus.md
│   ├── grafana.md
│   └── dashboards.md
│
├── logging/
│
├── security/
│
├── Dockerfile
├── .gitignore
└── README.md
```

---

# 🚀 Features

- Containerized application using Docker
- Kubernetes Deployment & Service
- Helm Chart deployment
- Rolling Update demonstration
- Helm Rollback demonstration
- GitHub Actions CI pipeline
- GitOps deployment using ArgoCD
- Prometheus monitoring
- Grafana dashboards
- Production-inspired project structure

---

# 🐳 Docker

Build Docker image

```bash
docker build -t pdfgenz-platformops-lab .
```

Run locally

```bash
docker run -p 8080:80 pdfgenz-platformops-lab
```

---

# ☸ Kubernetes

Deploy application

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

Rollback

```bash
helm rollback pdfgenz <revision>
```

View release history

```bash
helm history pdfgenz
```

---

# 🔄 GitHub Actions CI

The project includes a GitHub Actions workflow that demonstrates Continuous Integration by:

- Triggering on code push
- Building Docker images
- Validating project changes

Workflow location

```
.github/workflows/
```

---

# 🚀 GitOps with ArgoCD

ArgoCD continuously monitors the GitHub repository and synchronizes Kubernetes resources with the desired state stored in Git.

This demonstrates a GitOps workflow where Git acts as the single source of truth for deployments.

---

# 📊 Monitoring

## Prometheus

Prometheus collects Kubernetes metrics including:

- CPU
- Memory
- Node Health
- Pod Status
- Resource Utilization

---

## Grafana

Grafana visualizes metrics collected by Prometheus.

Example metrics include:

- CPU Usage
- Memory Usage
- Disk Usage
- Network Traffic
- Node Uptime

---

# 🔄 Rolling Updates

The project demonstrates Kubernetes Rolling Updates using Helm.

Application changes can be deployed with zero downtime by upgrading the Helm release.

---

# ↩ Rollback

Helm provides version history and instant rollback.

Example

```bash
helm rollback pdfgenz 3
```

---

# 📚 Skills Demonstrated

- Linux Administration
- Git & GitHub
- Docker
- Kubernetes
- Helm
- GitHub Actions
- GitOps
- ArgoCD
- Prometheus
- Grafana
- CI/CD Concepts
- Cloud-Native Deployment
- Infrastructure Automation

---

# 🔮 Future Enhancements

Potential future improvements include:

- Terraform Infrastructure as Code
- AWS EKS Deployment
- Horizontal Pod Autoscaler (HPA)
- Ingress Controller
- Centralized Logging (ELK/Loki)
- DevSecOps Security Scanning
- Trivy Container Scanning
- SonarQube Integration

---

# 👨‍💻 Author

**Syed Arif Ali**

Cloud & DevOps Engineer 
passionate about Kubernetes, Platform Engineering, Infrastructure Automation, Cloud Technologies, and AI-powered DevOps.

GitHub:
https://github.com/Syed-2050

---

# ⭐ If you found this project useful, consider giving it a star.

