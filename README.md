# 🚀 Cloud-Native Blog Platform (DevSecOps | Kubernetes | GitOps)

A cloud-native application demonstrating a complete **DevSecOps pipeline**, integrating CI/CD, container security, Kubernetes orchestration, and GitOps-based continuous delivery.

![Docker](https://img.shields.io/badge/Docker-Containerization-2496ED?style=flat-square&logo=docker)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-326CE5?style=flat-square&logo=kubernetes)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI/CD-2088FF?style=flat-square&logo=github-actions)
![ArgoCD](https://img.shields.io/badge/ArgoCD-GitOps-EF7B4D?style=flat-square&logo=argo)
![Terraform](https://img.shields.io/badge/Terraform-IaC-7B42BC?style=flat-square&logo=terraform)

---

## 🔐 DevSecOps Pipeline

- 🚀 CI/CD pipeline using **GitHub Actions**
- 🐳 Docker image build and version tagging
- 🧹 Dockerfile linting using **Hadolint**
- 🔍 Vulnerability scanning using **Trivy**
- 🔄 Automated image updates in Kubernetes manifests
- ⚙️ GitOps-based deployment using **ArgoCD**
- ☸️ Continuous sync between Git and Kubernetes cluster
- 🏗️ Infrastructure provisioning using **Terraform**

---

## 🏗️ Architecture
Source Code (GitHub)
↓
CI/CD Pipeline (GitHub Actions)
↓
Security Scanning (Hadolint + Trivy)
↓
Docker Image Build & Tagging
↓
Container Registry
↓
Kubernetes Cluster
↓
ArgoCD (GitOps Deployment)

---

## 📁 Project Structure
cloud-native-blog-platform/
├── .github/workflows/ # CI/CD pipelines
├── k8s/ # Kubernetes manifests
├── Terraform/ # Infrastructure as Code
├── backend/ # Backend service
├── frontend/ # Frontend service
├── deploy/ # Deployment scripts
├── docker-compose.yml
└── README.md

---

## ☸️ Kubernetes Deployment

- Containerized workloads deployed on Kubernetes
- Namespace-based isolation (`jerney`)
- Service-based communication between components
- Automated deployment via ArgoCD
- Continuous reconciliation with Git state

---

## 🔍 Troubleshooting & Real-World Issues

Handled production-like DevOps and Kubernetes issues:

- ❌ Invalid image references (**InvalidImageName**)  
- 📦 Image pull failures (**ImagePullBackOff**)  
- 🔁 Pod crashes (**CrashLoopBackOff**)  
- ⚙️ Init container failures  
- 🔌 Service misconfiguration (port/selector mismatch)  
- 🔐 Environment variable misconfiguration  
- 🗄️ Backend ↔ database connectivity issues  
- 📉 ArgoCD application health degradation  
- 🚨 CI/CD failures (image tagging/version mismatch)  

---

## 🔐 Security Practices

- Shift-left security in CI/CD pipeline  
- Automated vulnerability scanning before deployment  
- Docker image hardening and minimal base images  
- Continuous validation via GitOps workflow  
- Secure configuration using environment variables  

---

## 🌿 Branch Strategy

| Branch | Purpose |
|--------|--------|
| `main` | Source of truth for GitOps deployment and full DevSecOps pipeline |
---

## 🎯 Key Highlights

- End-to-end DevSecOps pipeline  
- Kubernetes-based deployment  
- GitOps delivery using ArgoCD  
- Integrated container security scanning  
- Real-world troubleshooting experience  

---

## 👨‍💻 Author

**Bijil Babu**  
DevSecOps | Kubernetes | Cloud Engineering  
