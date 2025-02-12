# Kubernetes Node.js Web UI Deployment
This repository contains a Node.js-based web UI deployed in Kubernetes using Minikube. The project demonstrates containerization with Docker, multi-image deployments, and Kubernetes configurations for managing a simple web application.
 
# Project Overview
# Tech Stack: Node.js, Docker, Kubernetes, Minikube
# key Concepts:
Creating and managing Docker images
Deploying multi-container applications in Kubernetes
Using Minikube for local cluster testing
Accessing the Minikube Dashboard to monitor deployments

# Setup & Installation
 # Ensure you have the following installed:

* Docker
* Kubernetes (kubectl)
* Minikube
* Node.js (for local testing)
* Git (for cloning this repository)

# Build & Push Docker Images
docker build -t my-node-app .

# Start Minikube
minikube start

# Deploy to Kubernetes
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

# Check Deployment
kubectl get pods
kubectl get services

# Access the Application
minikube dashboard
minikube service my-node-app --url

# Project Structure
📦 kubernetes-node-ui
 ┣ 📂 src
 ┃ ┣ 📜 app.js
 ┃ ┣ 📜 index.html
 ┣ 📜 Dockerfile
 ┣ 📜 deployment.yaml
 ┣ 📜 service.yaml
 ┣ 📜 README.md
 ┗ 📜 .gitignore
