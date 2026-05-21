# Deploy-a-Simple-Web-App-on-Kubernetes
Deploy a containerized web app into Kubernetes and expose it in the browser.

## Step 1: Install Required Tools

Install: To the your desktop

Docker Desktop

Minikube

kubectl

## Step 2: Start Kubernetes Cluster
minikube start
<img width="1188" height="202" alt="image" src="https://github.com/user-attachments/assets/b1ac33be-d858-4d90-949d-64a2d73bc22a" />

Check cluster:

kubectl get nodes
<img width="1350" height="154" alt="image" src="https://github.com/user-attachments/assets/bec839c5-5b78-487f-9f72-12f3e0955879" />

# Step 3: Create a Simple App

//create a simple app, example flask app.
//save the document app.py and another one requirements.txt. This tells Docker what Python packages to install.
//Code is added to the file section
<img width="454" height="246" alt="image" src="https://github.com/user-attachments/assets/a3f75a49-945d-434b-a883-0fc058242073" />

## Step 4: Create Dockerfile
//You’ll create a Docker container for your Flask app so Kubernetes can run it.
<img width="569" height="400" alt="image" src="https://github.com/user-attachments/assets/36f730e8-d6f8-41bd-a722-7e16429ecec6" />




