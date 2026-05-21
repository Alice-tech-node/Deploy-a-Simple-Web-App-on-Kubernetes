# Deploy-a-Simple-Web-App-on-Kubernetes
*Deploy a containerized web app into Kubernetes and expose it in the browser.*

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
/*create a simple app, example flask app, save the document app.py and another one requirements.txt.*

/*This tells Docker what Python packages to install. Code is added to the file section*
<img width="454" height="246" alt="image" src="https://github.com/user-attachments/assets/a3f75a49-945d-434b-a883-0fc058242073" />

## Step 4: Create Dockerfile
/*You’ll create a Docker container for your Flask app so Kubernetes can run it.*
> FROM python:3.11 - Uses Python 3.11 image.
> WORKDIR /app - Creates /app inside container.
> COPY . . - Copies everything from your folder into container.
> RUN pip install -r requirements.txt - Installs Flask.
> EXPOSE 5000 - Allows access to app on port 5000.
> CMD ["python", "app.py"] - Runs your app when container starts.

<img width="584" height="400" alt="image" src="https://github.com/user-attachments/assets/cd84b794-f3ae-48ad-b856-7a4fe0ee1cfd" />

## Step 5: Build Docker Image
*The docker image is created by using this command;docker build -t flask-k8s-app .*

> docker build → build image

> -t → tag/name image

> . → current folder






