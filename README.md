🚀 Build a Kubernetes Cluster Locally with Minikube

📌 Project Overview

This project demonstrates how to set up and manage a local Kubernetes cluster using Minikube. It covers cluster initialization, deploying applications, exposing services, scaling workloads, and basic monitoring. The goal is to understand container orchestration in a practical DevOps environment.

🛠️ Tech Stack

Kubernetes

Minikube

Docker

kubectl

YAML

🎯 Objectives

Install and configure Minikube

Create a local Kubernetes cluster

Deploy applications using YAML manifests

Expose services (NodePort / ClusterIP)

Scale deployments

Monitor cluster resources

⚙️ Prerequisites

Make sure you have installed:

Docker

Minikube

kubectl

🚀 Setup & Execution Steps

1️⃣ Start Minikube
minikube start

2️⃣ Check Cluster Status
kubectl cluster-info
kubectl get nodes

3️⃣ Create a Deployment
kubectl create deployment nginx --image=nginx


Or apply YAML file:

kubectl apply -f deployment.yaml

4️⃣ Expose the Deployment
kubectl expose deployment nginx --type=NodePort --port=80

5️⃣ Access the Service
minikube service nginx

6️⃣ Scale the Deployment
kubectl scale deployment nginx --replicas=3

📊 Useful Commands
kubectl get pods
kubectl get services
kubectl describe pod <pod-name>
kubectl logs <pod-name>

📂 Project Structure
.
├── deployment.yaml
├── service.yaml
└── README.md

📸 Screenshots

(Add screenshots of cluster running, pods, and services here)

🎓 Learning Outcomes

Understanding Kubernetes architecture

Working with Pods, Deployments, and Services

Managing containerized applications

Hands-on DevOps practice

📜 License

This project is licensed under the MIT License.
