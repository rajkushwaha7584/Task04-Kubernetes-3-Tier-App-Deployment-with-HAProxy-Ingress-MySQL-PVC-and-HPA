#Add HAProxy Ingress setup for Task04 Kubernetes deployment

## HAProxy Ingress Setup

In this task, the existing NGINX Ingress setup was replaced with HAProxy Ingress Controller.

### Changes Implemented

- Updated `ingressClassName` from `nginx` to `haproxy`
- Removed the old NGINX Ingress Controller
- Installed HAProxy Ingress Controller using Helm
- Updated Ingress routing rules
- Verified application routing for:
  - `/` → Frontend Service
  - `/api` → Backend Service
  - `/health` → Backend Service

### Final Traffic Flow

Browser → HAProxy Ingress Controller → Ingress Rules → Frontend/Backend Service → Pods → MySQL Service → MySQL Pod with PVC


#-->
Completed Task04 Kubernetes 3-tier application deployment with HAProxy Ingress.

In this project, I deployed a frontend, backend API, and MySQL database on a Kind Kubernetes cluster. I configured Kubernetes resources including Deployment, StatefulSet, Service, Secret, ConfigMap, PVC, Ingress, and HPA.

I also replaced the NGINX Ingress Controller with HAProxy Ingress Controller using Helm. The final routing flow sends `/` traffic to the frontend service, while `/api` and `/health` traffic are routed directly to the backend service.

This task helped me understand Kubernetes networking, Ingress controllers, service-to-pod communication, persistent storage, and autoscaling.
