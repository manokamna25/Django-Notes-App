# 📝 NotesApp: Full-Stack Hub with DevOps Pipeline

[![Django](https://img.shields.io/badge/Django-4.1.5-092E20?style=for-the-badge&logo=django&logoColor=white)](https://www.djangoproject.com/)
[![React](https://img.shields.io/badge/React-2023-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-Enabled-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)](https://kubernetes.io/)
[![Jenkins](https://img.shields.io/badge/Jenkins-CI%2FCD-D24939?style=for-the-badge&logo=jenkins&logoColor=white)](https://www.jenkins.io/)

A modern, fast, and professional notes-taking application built with **Django REST Framework** and **React.js**. This project isn't just a simple app; it's a **complete DevOps showcase** including containerization, CI/CD pipelines, and orchestration.

---

## ✨ Features

- **Full CRUD Operations**: Create, read, update, and delete notes instantly.
- **Modern UI/UX**: Clean, responsive interface with a sleek **Dark Mode** toggle.
- **RESTful API**: Robust backend powered by Django REST Framework.
- **DevOps Ready**: 
  - 🐋 **Dockerized**: Simplified setup with Docker and Docker Compose.
  - ⚓ **Kubernetes**: Production-ready manifests for orchestration.
  - 🚀 **Automation**: Pre-configured `Jenkinsfile` for CI/CD pipelines.

---

## 🛠️ Tech Stack

### Backend
- **Core**: Django 4.1.5
- **API**: Django REST Framework
- **Database**: SQLite (Development) / PostgreSQL (Ready)
- **Static Hosting**: WhiteNoise

### Frontend
- **Framework**: React.js
- **Routing**: React Router DOM (HashRouter)
- **Styling**: Vanilla CSS (Custom Variable System)

### Infrastructure
- **Containerization**: Docker & Docker Compose
- **Orchestration**: Kubernetes (K8s)
- **CI/CD**: Jenkins
- **Reverse Proxy**: Nginx

---

## 🚀 Getting Started

### 1. Local Development (Manual)

#### Backend Setup
```bash
# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py makemigrations
python manage.py migrate

# Start server
python manage.py runserver
```

#### Frontend Setup
```bash
cd mynotes
npm install
npm start
```

---

### 2. Docker Setup (Recommended)

```bash
# Build and Run with Docker Compose
docker-compose up --build
```
*Access the app at `http://localhost:8000`*

---

### 3. Kubernetes Deployment

```bash
# Create the namespace
kubectl apply -f notes-app/namespace.yml

# Deploy the application
kubectl apply -f notes-app/deployment.yml

# Expose via service
kubectl apply -f notes-app/service.yml
```

---

## 🏗️ Project Structure

```text
├── api/                # Django REST API App
├── notesapp/           # Django Project Core
├── mynotes/             # React Frontend
├── staticfiles/        # Compiled Static Files
├── Dockerfile          # Container Config
├── docker-compose.yml  # Multi-container Config
├── Jenkinsfile         # CI/CD Pipeline
└── notes-app/          # K8s Manifests
```

---

## 🔧 Jenkins Pipeline

The project includes a `Jenkinsfile` that automates:
1.  **Code Checkout**: Pulls latest code from Git.
2.  **Building**: Builds Docker images for the app.
3.  **Testing**: Ready for unit tests (Django/React).
4.  **Deployment**: Pushes to your registry and updates K8s.

---

## 🤝 Contributing

Contributions are welcome! If you have suggestions or want to improve the app:
1. Fork the repo.
2. Create a feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes.
4. Push to the branch and open a Pull Request.

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

> [!TIP]
> **Pro Tip**: To truly make this "khaas", don't forget to add screenshots of the running app in this section!

---

*Project by [Your Name]*
