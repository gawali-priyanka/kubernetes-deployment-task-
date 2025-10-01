## Kubernetes Deployment with Minikube
---
## Task-5
---
This repository contains the deployment of a Python-based web application using Kubernetes on a local Minikube cluster. The app serves a static HTML page and demonstrates core Kubernetes concepts like Deployments, Services, and Pod scaling.

Files Included <br>
├── screenshots/ <br>
├── deployment.yaml <br>
├── service.yaml <br>

## Tools & Technologies
1) Docker
2) Kubernetes
3) Minikube
4) kubectl
----

## How to Run This Project
1. Start Minikube
   minikube start
2. Build the Docker Image
   docker build -t my-kube-app:v1 .
3. Deploy the Application to Kubernetes
   kubectl apply -f deployment.yaml
4. Expose the Deployment using a LoadBalancer Service
   kubectl apply -f service.yaml
5. Access the Web Application
   minikube service my-kube-app-service
---
## Kubernetes Commands Used
 kubectl get pods <br>
 kubectl get svc <br>
 kubectl describe pod <pod-name> <br>
 kubectl logs <pod-name> <br>
 kubectl scale deployment my-kube-app --replicas=2 <br>
 ---
 ## Screenshots
 ---
 Pods
![Branches](https://github.com/gawali-priyanka/kubernetes-deployment-task-/blob/main/screenshots/pods.png?raw=true)
 ----
 Deployment
 ----
![Branches](https://github.com/gawali-priyanka/kubernetes-deployment-task-/blob/main/screenshots/deployment.png?raw=true)
-----
 Pod logs
----
![Branches](https://github.com/gawali-priyanka/kubernetes-deployment-task-/blob/main/screenshots/pod-loges.png?raw=true)
-----
Replicas of pods
-----
![Branches](https://github.com/gawali-priyanka/kubernetes-deployment-task-/blob/main/screenshots/Replicas-pods.png?raw=true)
