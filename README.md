# Project Source Code 🚀

This is my **final bootcamp project**, where I implemented a full CI/CD pipeline with Jenkins, Docker, and Kubernetes.  
The project demonstrates how to build, containerize, and deploy a Java-based application in a production-like environment.  

---

## 📌 Features
- Java application built with Maven (`pom.xml`)
- Containerized using Docker
- Kubernetes manifests (`deployment.yaml`) for deployment
- CI/CD pipeline configured with **Jenkinsfile**
- SonarCloud integration for code quality
- Configurable application port

---

## 🛠️ Tech Stack
- **Java 17**
- **Maven**
- **Docker**
- **Kubernetes**
- **Jenkins**
- **SonarCloud**

---

## ⚙️ How It Works
1. Code is pushed to GitHub.
2. Jenkins pipeline:
   - Builds the project using Maven
   - Runs tests
   - Runs SonarCloud analysis
   - Builds & pushes Docker image
   - Deploys to Kubernetes cluster using `deployment.yaml`

---

## 🚀 Deployment
- Dockerized app can be run locally:
  ```bash
  docker build -t myapp .
  docker run -p 8080:8080 myapp
