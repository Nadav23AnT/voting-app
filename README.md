# Voting-app (Kubernetes implementation ) [KodeKloud DevOps course - project]
This is based on the original example-voting-app repository from the docker-examples GitHub page
and modified to work on the Kubernetes cluster.
## Illustration of the app

![voting-app-deployment-map](https://github.com/Nadav23AnT/voting-app/assets/71144691/fea61d25-7ee1-46de-a864-af9d1fa03c8d)
## Goals:


1. Deploy PODs
2. Enable connectivity between containers
3. Add External Access
### Use Kubectl on the terminal
Start Voting-App
```bash
kubectl create -f voting-app-deploy.yaml
kubectl create -f voting-app-service.yaml
```
Start Redis
```bash
kubectl create -f redis-deploy.yaml
kubectl create -f redis-service.yaml
```
Start Postgres
```bash
kubectl create -f postgres-deploy.yaml
kubectl create -f postgres-service.yaml
```
you can check the pods and services using:
```bash
kubectl get all
```
![map-voting-app](https://github.com/Nadav23AnT/voting-app/assets/71144691/6fd98eca-5cd5-4a4d-872a-eaa1401f8d3d)
