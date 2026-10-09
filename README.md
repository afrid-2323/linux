# Kubernetes Web Application Deployment

## Project Overview

Deployed an Nginx web application on a Kubernetes cluster running on an AWS EC2 instance.

## Technologies Used

* AWS EC2
* Ubuntu Linux
* Kubernetes
* kubectl
* Nginx
* YAML
* Git and GitHub

## Project Features

* Deployed Nginx using a Kubernetes Deployment.
* Configured five application replicas.
* Exposed the application using a NodePort Service.
* Tested Kubernetes self-healing by deleting a Pod.
* Scaled the application from three replicas to five.
* Performed a rolling update and rollback.
* Verified application availability using curl.

## Deployment Commands

Apply the Deployment:

```bash
kubectl apply -f deployment.yaml
```

Apply the Service:

```bash
kubectl apply -f service.yaml
```

Check Pods:

```bash
kubectl get pods -l app=k8s-webapp
```

Check the Deployment:

```bash
kubectl get deployment k8s-webapp
```

Scale the application:

```bash
kubectl scale deployment k8s-webapp --replicas=5
```

Check the Service:

```bash
kubectl get service k8s-webapp-service
```

Test the application:

```bash
curl http://localhost:30080
```

## What I Learned

* Kubernetes Deployments and ReplicaSets
* Pods and container management
* NodePort Services
* Scaling applications
* Kubernetes self-healing
* Rolling updates and rollbacks
* Basic application troubleshooting
