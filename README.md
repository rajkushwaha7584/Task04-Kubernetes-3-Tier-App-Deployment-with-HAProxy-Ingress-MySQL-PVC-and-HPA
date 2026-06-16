# Task04-3-Tier-Application-Deployment-on-Kubernetes-Kind-with-Ingress-MySQL-PVC-and-HPA
# Task04: Kubernetes 3-Tier Application Deployment

This project is a Kubernetes-based deployment of a 3-tier application using Kind cluster.

## Project Components

- Frontend application running with Nginx
- Backend API service
- MySQL database
- Kubernetes Ingress for browser access
- ClusterIP services for internal communication
- StatefulSet and PVC for database persistence
- HPA for backend auto-scaling

## Architecture Flow

Browser → Ingress → Frontend Service → Frontend Pod → Backend Service → Backend Pod → DB Service → MySQL Pod → PVC

## What I Learned

- How to deploy frontend, backend, and database on Kubernetes
- How services communicate internally using ClusterIP
- How Ingress exposes the application to browser
- How StatefulSet and PVC are used for database persistence
- How HPA scales backend pods based on CPU usage
# Task04-Kubernetes-3-Tier-App-Deployment-with-HAProxy-Ingress-MySQL-PVC-and-HPA
