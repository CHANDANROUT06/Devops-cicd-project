Devops CI/CD Docker project 



This project demonstrates a **basic CI/CD pipeline** using **GitHub, Jenkins, Docker**, and a simple web application.

---
 Project Overview

- Source code hosted on **GitHub**
- Automated build triggered by **Jenkins**
- Application containerized using **Docker**
- Jenkins builds Docker image and runs container automatically

---

 Tech Stack Used

- Git & GitHub
- Jenkins (CI/CD)
- Docker
- Linux (Ubuntu / WSL)
- HTML (Simple Web App)

---
 Project Flow (CI/CD)

1. Developer pushes code to GitHub
2. Jenkins pulls latest code from repository
3. Jenkins builds Docker image
4. Docker container runs the application
5. Application is accessible via browser

---

 Project Structure

```text
Devops-cicd-project/
├── Dockerfile
├── index.html
├── README.md
