## **Full Stack Realtime Chat App 🚀**

## 📘 Overview
This project delivers a scalable, secure, and real-time chat application using modern DevOps practices. Designed for seamless user experience and ease of deployment, it integrates the latest technologies in development and operations.

## 🛠️ Tech Stack
* Backend: Node.js, Express, MongoDB, Socket.io
* Frontend: React, TailwindCSS
* Containerization: Docker
* Orchestration: Kubernetes (planned)
* Authentication: JWT
* State Management: Zustand
* Web Server: Nginx

## 🚀 Features
* Real-time messaging with Socket.io
* Secure user authentication using JWT
* Dockerized for seamless deployment
* Scalable architecture with Kubernetes integration (coming soon)
* Modern UI with React & TailwindCSS
* Easy profile management and online status updates

## 🔧 Prerequisites
* Node.js (v14 or higher)
* Docker
* Git

## 📦 Setup & Deployment
Clone the Repository
  ```
  git clone https://github.com/iemafzalhassan/full-stack_chatApp.git
  cd full-stack_chatApp
  ```
Docker Compose Deployment
  ```
  docker-compose up -d --build
  Access the app at: http://localhost
  ```

## 🏗️ Manual Docker Deployment
Create a Docker Network
  ```
  docker network create full-stack
  ```
Run MongoDB
  ```
  docker run -d -p 27017:27017 --name mongo mongo:latest
  ```
Build & Run Backend
  ```
  cd backend
  docker build -t full-stack_backend .
  docker run -d --network=full-stack -p 5001:5001 --env-file .env full-stack_backend
  ```
Build & Run Frontend
  ```
  cd frontend
  docker build -t full-stack_frontend .
  docker run -d --network=full-stack -p 5173:5173 --name frontend full-stack_frontend:latest
  Access frontend at: http://localhost:5173
  ```

## 🔍 Monitoring & Logging
Use the following command to monitor logs and troubleshoot:
  ```
  docker-compose logs -f
  ```

## 📚 Project Snapshots:

![image](https://github.com/user-attachments/assets/eb766945-dc3e-4524-8691-a46831e8df61)

![image](https://github.com/user-attachments/assets/6e96469d-a93c-4359-8131-5a61aa6ec275)

![WhatsApp Image 2025-02-01 at 01 56 39_32fc5c56](https://github.com/user-attachments/assets/63598cc6-731e-4113-b4ed-59dfaccb1f2f)

