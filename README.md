# Vue.js Application Deployment Using Docker

This repository contains a **Vue.js application containerized using Docker**.
It supports both **development and production builds**, making it easy to build,
run, and deploy a Vue.js application in a consistent environment.

---

## 🚀 Tech Stack

- Vue.js
- JavaScript
- HTML & CSS
- Docker
- Node.js
- Nginx (for production build)

---

## 📂 Project Structure

```
.
├── public/                 # Public static files
├── src/                    # Vue.js source code
├── .dockerignore           # Docker ignore rules
├── .gitignore              # Git ignore rules
├── Dockerfile              # Development Dockerfile
├── Dockerfile-prod         # Production Dockerfile
├── babel.config.js         # Babel configuration
├── package.json            # Project dependencies
├── package-lock.json       # Dependency lock file
├── vue.config.js           # Vue configuration
└── README.md
```

---

## ⚙️ Prerequisites

Ensure the following are installed:

- Docker
- Node.js (optional, only if running locally without Docker)

Check Docker:
```bash
docker --version
```

---

## 🛠️ Development Setup (Docker)

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Hritickjha/Vue.Js-application-and-deploy-using-Docker.git
cd Vue.Js-application-and-deploy-using-Docker
```

### 2️⃣ Build Docker Image
```bash
docker build -t vue-app-dev .
```

### 3️⃣ Run Development Container
```bash
docker run -p 8080:8080 vue-app-dev
```

---

## 🌐 Access Application

- Vue App (Development): http://localhost:8080

---

## 🏗️ Production Build Using Docker

### 1️⃣ Build Production Image
```bash
docker build -f Dockerfile-prod -t vue-app-prod .
```

### 2️⃣ Run Production Container
```bash
docker run -p 80:80 vue-app-prod
```

---

## 📦 Common Docker Commands

```bash
docker ps                    # List running containers
docker images                # List images
docker stop <container_id>   # Stop container
docker rm <container_id>     # Remove container
docker rmi <image_id>        # Remove image
```

---

## 🧪 Run Locally Without Docker (Optional)

```bash
npm install
npm run serve
```

Production build:
```bash
npm run build
```

---

## ✅ Features

- Vue.js single-page application
- Dockerized development environment
- Production-ready Docker build
- Lightweight and portable deployment
- Easy to scale and deploy anywhere

---

## 📌 Use Cases

- Learning Docker with Vue.js
- Frontend deployment practice
- DevOps / frontend portfolio project
- CI/CD-ready containerized frontend app

---

## 👤 Author

Hritick Jha  
GitHub: https://github.com/Hritickjha

---

## 📄 License

This project is open-source and available under the MIT License.
