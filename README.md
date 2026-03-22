# 🚀 Inventory Kubernetes Deployment

Production-ready Kubernetes deployment for a containerized ASP.NET Core Web API with SQL Server.

---

## 🧱 Architecture

- ASP.NET Core Web API (Dockerized)
- SQL Server (containerized)
- Kubernetes (local cluster)
- NGINX Ingress Controller

---

## ⚙️ Tech Stack

- .NET 8
- Docker
- Kubernetes (k8s)
- SQL Server
- NGINX Ingress

---

## 📁 Project Structure

k8s/
├── namespace.yaml      # Namespace definition  
├── deployment.yaml     # API deployment  
├── service.yaml        # Internal service  
├── ingress.yaml        # External access via NGINX  
└── sqlserver.yaml      # SQL Server pod  

---

## 🚀 How to Run

### 1. Apply Kubernetes configs

kubectl apply -f k8s/

### 2. Verify resources

kubectl get pods -n inventory-app  
kubectl get svc -n inventory-app  

---

## 🌐 Access API

Add to `/etc/hosts`:

127.0.0.1 inventory.local  

Then open:

http://inventory.local  

---

## 📌 Features

- Containerized microservice architecture  
- Kubernetes deployment with namespace isolation  
- Internal service communication  
- External access via Ingress  
- SQL Server integration  

---

## 📷 Notes

This project demonstrates real-world DevOps practices including container orchestration and service exposure using Kubernetes.

---

## 👨‍💻 Author

Usman 