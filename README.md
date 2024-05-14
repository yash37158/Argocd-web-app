# React Web Application Deployment with Argo CD and Argo Rollouts

This project demonstrates a GitOps workflow for deploying a simple React web application to a Kubernetes cluster using Argo CD and Argo Rollouts.

## Prerequisites

- Kubernetes cluster (Minikube, kind, or a cloud provider's Kubernetes service)
- Docker and Git installed
- Argo CD and Argo Rollouts installed on your cluster

## Project Structure

```plaintext
react-app/
├── manifests/
│   ├── deployment.yaml
│   ├── service.yaml
│   └── rollout.yaml
├── Dockerfile
├── README.md
├── package.json
└── other React project files...
```
## Steps Completed

- Dockerizing the React Application
- Pushing Docker Image to Docker Hub
- Creating Kubernetes Manifests
- Pushing Code to GitHub
- Installing Argo CD
- Creating an Argo CD Application
- Syncing and Monitoring the Application

## ScreenShot
![Screenshot 2024-05-15 at 12 09 38 AM](https://github.com/yash37158/Argocd-web-app/assets/68152307/266ddd1b-9fc8-44ef-8cd4-b45eddc66deb)

## CleanUp
To remove resources:
- kubectl delete application react-app -n argocd
- kubectl delete namespace argocd
- kubectl delete namespace argo-rollouts





