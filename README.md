# Kubernetes Deployment Project

## Objective
Deploy a microservices-based application on Kubernetes cluster.

## Technologies Used
- Docker
- Kubernetes
- Python Flask
- Nginx
- VS Code

## Project Structure

kubernetes_project/
│
├── backend/
├── frontend/
├── k8s/

## Backend
Flask API returning JSON response.

## Frontend
Simple HTML page served using Nginx.

## Kubernetes Files
- backend-deployment.yaml
- backend-service.yaml
- frontend-deployment.yaml
- frontend-service.yaml

## Commands Used

docker build -t backend-app ./backend
docker build -t frontend-app ./frontend

kubectl apply -f k8s/backend-deployment.yaml
kubectl apply -f k8s/backend-service.yaml
kubectl apply -f k8s/frontend-deployment.yaml
kubectl apply -f k8s/frontend-service.yaml

kubectl get pods
kubectl get svc

## Output
Application deployed successfully on Kubernetes cluster.  
<img width="1913" height="969" alt="Image" src="https://github.com/user-attachments/assets/5c3f5a16-17f2-4bab-a701-fda56a2d7139" />
<img width="1920" height="964" alt="Image" src="https://github.com/user-attachments/assets/ba3aa59b-a651-4adb-8d2b-f2ec2f86e765" />
