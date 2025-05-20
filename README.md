# 📝 Task Tracker App

A full-stack Task Tracker application with Dockerized frontend and backend, local development support using `docker-compose`, and a CI pipeline using GitHub Actions. Built and maintained with DevOps best practices.

---

## 📦 Project Structure

```bash
.
├── frontend/              # React frontend
│   └── Dockerfile
├── backend/               # Express backend
│   └── Dockerfile
├── docker-compose.yml     # Local development setup
└── .github/workflows/
    └── ci.yml             # GitHub Actions CI workflow
```

---

## 🚀 Features

- 🐳 Dockerized frontend and backend
- 🔧 Local development with `docker-compose`
- ✅ CI pipeline with GitHub Actions
- ☁️ Deployment-ready for AWS (ECS or EC2)
- 📈 (Optional) Monitoring with Grafana/Prometheus
- 🌐 (Optional) Staging and production environments

---

## 🛠️ Getting Started

### Prerequisites

- Docker & Docker Compose installed
- Node.js installed (if testing outside Docker)
- GitHub account

---

## 🐳 Local Development

1. Clone the repository:

```bash
git clone https://github.com/your-username/task-tracker-app.git
cd task-tracker-app
```

2. Run the app locally with Docker Compose:

```bash
docker-compose up --build
```

3. App runs at:

- Frontend: `http://localhost:3000`
- Backend: `http://localhost:5000`

---

## 🔁 CI Pipeline (GitHub Actions)

CI pipeline is triggered on push or PR to `main` branch. It performs the following:

- ✅ Checkout code
- 🔧 Build Docker images for frontend and backend
- 🧪 Run tests (if defined)
- 🔐 Optionally pushes images to DockerHub

Path: `.github/workflows/ci.yml`

To enable DockerHub image pushing, add the following **repository secrets**:

- `DOCKERHUB_USERNAME`
- `DOCKERHUB_TOKEN`

---

## ☁️ Deployment (AWS – optional)

Deployment can be done via:

- AWS ECS using pushed Docker images
- AWS EC2 with manual setup
- (GitHub Actions can be extended for automatic deployment)

*Deployment link will be provided upon deployment.*

---

## 🎁 Bonus (Planned)

- 📊 Monitoring with Prometheus and Grafana
- 🧪 Staging and production environments with separate pipelines

---

## 📸 Deliverables

- ✅ GitHub repository: [Repo Link](https://github.com/your-username/task-tracker-app)
- 🌍 Deployment Link: _Coming soon_
- 📋 CI Pipeline Logs: _Available in GitHub Actions tab_

---

## 👨🏽‍💻 Author

Temi – Cloud Infrastructure Engineer & DevOps Enthusiast  
GitHub: [@your-username](https://github.com/your-username)

---

## 📄 License

This project is licensed under the MIT License.