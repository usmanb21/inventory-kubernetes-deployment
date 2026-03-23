# 🚀 Inventory Kubernetes Deployment

Production-style Kubernetes deployment for a containerized ASP.NET Core Web API with SQL Server.

---

## 🏗️ Architecture

Client → Ingress → Service → API Pod → SQL Server Pod

---

## 📦 Components

- ASP.NET Core Web API (Dockerized)
- SQL Server (containerized)
- Kubernetes (local cluster)
- NGINX Ingress Controller

---

## 📁 Project Structure

```
k8s/
  namespace/
  api/
  database/
  ingress/
```

---

## ⚙️ Deployment Steps

```bash
kubectl apply -f k8s/namespace/
kubectl apply -f k8s/database/
kubectl apply -f k8s/api/
kubectl apply -f k8s/ingress/
```

---

## 🌐 Access

Add to /etc/hosts:

```
127.0.0.1 inventory.local
```

Then open:

http://inventory.local

---

## 🛠️ Tech Stack

- Kubernetes
- Docker
- ASP.NET Core (.NET 8)
- SQL Server
- NGINX Ingress

---

## 📌 Notes

- Uses ClusterIP service for internal communication
- Ingress routes external traffic
- Environment variables used for DB connection
