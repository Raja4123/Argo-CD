# 🚀 GitOps Kubernetes Deployment on AWS (KOPS + Argo CD + Monitoring)

## 1. About the Project

This project demonstrates a **GitOps-based Kubernetes deployment** on AWS.

- Kubernetes cluster is created using **KOPS**
- Application is deployed using **Deployment and Service**
- **Argo CD** automatically syncs application changes from GitHub to Kubernetes
- **Prometheus** collects metrics
- **Grafana** provides monitoring dashboards

### Flow
Developer → GitHub → Argo CD → Kubernetes Cluster → Website  
Monitoring → Prometheus → Grafana

The goal of this project is to automate deployments and implement a production-style DevOps workflow.

---

## 2. Advantages of This Project

### Before (Manual Process)
- Manual login to server
- Run `kubectl apply`
- No deployment history
- High chance of human errors
- Difficult rollback

### After (GitOps)
- Push changes to GitHub → Automatic deployment
- Git becomes the **Single Source of Truth**
- Automatic sync with Kubernetes
- Easy rollback using Git
- Faster and reliable deployments
- Real-time monitoring of cluster and application
- Production-ready DevOps workflow

---

## 3. Prerequisites / Required Tools

Make sure the following tools are installed:

- AWS Account
- AWS CLI
- kubectl
- KOPS
- Docker
- Git
- Helm (Prometheus, Grafana)
- S3 bucket (for KOPS state store)

