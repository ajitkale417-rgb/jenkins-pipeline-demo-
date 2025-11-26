# Three-Tier Application on AWS EKS

This repository contains Kubernetes manifests and application code for deploying a simple 3-tier architecture on Amazon EKS.

## Architecture
- **Frontend:** Nginx (static HTML)
- **Backend:** Node.js Express API
- **Database:** MySQL (with PVC for persistence)

## Folder Structure
- `backend/` – Node.js API source and Dockerfile
- `frontend/` – Static HTML + Dockerfile for Nginx
- `k8s/` – Kubernetes deployment YAML files (MySQL, backend, frontend)

## Steps to Deploy
1. Create an EKS cluster  
2. Build and push Docker images  
3. Apply Kubernetes manifests  
4. Access frontend via LoadBalancer external IP  

Refer to `k8s/` directory for manifests and detailed instructions.
