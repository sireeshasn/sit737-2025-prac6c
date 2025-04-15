# sit737-2025-prac6c
# SIT737-2025 Practical Task 6C: Interacting with Kubernetes

## 👩‍💻 Overview

This task demonstrates how to interact with a Kubernetes cluster using `kubectl`, deploy and update a Node.js microservice, and verify the functionality via the Kubernetes Dashboard and port-forwarding.

---

## 🧰 Tools Used

- **GitHub** – Source code hosting and version control  
- **Visual Studio Code** – Code editor  
- **Node.js** – JavaScript runtime for the backend app  
- **Docker** – Containerization platform  
- **Docker Hub** – Image registry  
- **Kubernetes** – Cluster orchestration platform  
- **kubectl** – Kubernetes CLI  

---

## 🚀 Project Structure


calculator-microservice/ │ ├── app.js # Express backend app ├── Dockerfile # Docker build configuration ├── package.json # Node.js dependencies ├── deployment.yaml # Kubernetes Deployment config ├── service.yaml # Kubernetes Service config └── README.md # Project documentation
## 🔧 Part I – Interacting with the Cluster

### ✅ Check Pods and Services

```bash
kubectl get pods
kubectl get services
kubectl port-forward service/node-app-service 3000:3000
http://localhost:3000

**Modify app.js**
res.send('Hello from the UPDATED Node.js App!');
