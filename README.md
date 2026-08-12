# 🚀 Web Application Deployment on K3s with AWS EC2

## 📌 Project Overview

I recently completed a hands-on deployment where I **containerized a web application using Docker** and deployed it on a **K3s Kubernetes cluster running on an AWS EC2 instance**.

## 🛠️ Technologies Used

* ☁️ **AWS EC2** – Hosting the K3s cluster
* 🐳 **Docker** – Containerizing the application
* 📦 **Docker Hub** – Storing and pulling Docker images
* ☸️ **K3s / Kubernetes** – Deploying and managing the application
* 🚀 **Kubernetes Deployment** – Managing application workloads
* 🌐 **Kubernetes Service** – Application networking
* 🔀 **NGINX Ingress Controller** – Exposing the application externally
* 🌍 **GoDaddy DNS** – Connecting the domain to the EC2 instance
* 🔧 **Git & GitHub** – Version control and project management

## 🔄 Deployment Flow

```text
Application
     ↓
Docker Image
     ↓
Docker Hub
     ↓
K3s Cluster on AWS EC2
     ↓
Kubernetes Deployment
     ↓
Kubernetes Service
     ↓
NGINX Ingress Controller
     ↓
Domain 🌐
```

## 🧩 What I Learned

During the deployment, I faced and resolved a **port configuration issue**, which helped me understand how the following Kubernetes networking concepts work together:

* `containerPort`
* `targetPort`
* Service `port`
* Ingress port

This project gave me practical experience with:

* Containerization
* Kubernetes deployments
* Kubernetes networking
* K3s
* AWS infrastructure
* NGINX Ingress
* DNS configuration
* Docker image management

## 🎯 Key Takeaway

This project strengthened my understanding of **deploying containerized applications on Kubernetes in a real cloud environment** and gave me valuable hands-on experience with AWS, Docker, K3s, and Kubernetes networking.

> Still learning, still building, and getting one step closer to becoming a **Cloud & DevOps Engineer**. ☁️🚀
