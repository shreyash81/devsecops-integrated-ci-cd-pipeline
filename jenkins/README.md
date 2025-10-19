# 🎮 Jenkins DevSecOps Tic Tac Toe Automation

![Tic Tac Toe Screenshot](screenshot-link-here)

This project demonstrates **end-to-end DevSecOps automation** for a Tic Tac Toe game using **Jenkins, Docker, Kubernetes, Helm, and Argo CD**.  
The pipeline handles **build, test, containerization, security scanning, and automated deployment** to Kubernetes.

---

## 🛠 Features

- Fully functional **Tic Tac Toe game** with **X, O, and Draw** tracking  
- **Game history** with timestamps and highlights winning combinations  
- **Responsive design** for all devices  
- **Jenkins pipeline** automates: build → test → Docker image → deploy  
- **Security integration** with **Trivy, Snyk, and SonarQube**  
- Deployment on **Kubernetes cluster** using **Helm & Argo CD**  
- Health checks and HPA for **production-ready scalability**

---

## 🧰 Technologies Used

- **Frontend:** React 18, TypeScript, Tailwind CSS, Lucide React (icons)  
- **CI/CD & DevSecOps:** Jenkins, Docker, Kubernetes, Helm, Argo CD  
- **Security & Quality:** Trivy, Snyk, SonarQube  

---

## 📂 Project Structure

src/
├── components/
│ ├── Board.tsx # Game board component
│ ├── Square.tsx # Individual square component
│ ├── ScoreBoard.tsx # Tracks X, O, and Draw scores
│ └── GameHistory.tsx # Tracks game history with timestamps
├── utils/
│ └── gameLogic.ts # Game logic utilities
├── App.tsx # Main application component
└── main.tsx # Entry point
jenkins/
└── Jenkinsfile # Full CI/CD pipeline
kubernetes/
└── deployment.yaml # Kubernetes deployment manifest

yaml
Copy code

---

## 🚀 Jenkins CI/CD Pipeline

1. **Code push** triggers Jenkins pipeline  
2. **Static code analysis** with SonarQube  
3. **Security scans** with Trivy and Snyk  
4. **Docker image** built and pushed to registry  
5. **Kubernetes deployment** automated via Helm & Argo CD  
6. **HPA, health checks**, and monitoring ensure **reliable production-grade uptime**  

---

## ⚡ Getting Started

### Prerequisites

- Node.js (v14+), npm or yarn  
- Docker  
- Kubernetes cluster with `kubectl` access  
- Jenkins server configured for pipeline execution  

### Installation

```bash
git clone https://github.com/shreyash81/devsecops-tictactoe.git
cd devsecops-tictactoe
npm install       # or yarn install
npm run dev       # or yarn dev
Open your browser: http://localhost:5173

Build & Deployment
bash
Copy code
npm run build
docker build -t tictactoe-app:latest .
kubectl apply -f kubernetes/deployment.yaml
📈 Pipeline Highlights
End-to-end automation with Jenkins from code commit → deploy

Security scans integrated into CI/CD pipeline

GitOps deployment using Helm & Argo CD

Scalable & resilient deployment with HPA, health checks, and monitoring

📌 About
This project is a hands-on example of DevSecOps for full-stack applications:

Automation of build, test, security scanning, and deployment

Production-ready deployment using Kubernetes, Helm, and Argo CD

Fast rollbacks and maintainable CI/CD pipelines

Focused entirely on Jenkins-driven DevSecOps practices

🔖 Topics
react typescript jenkins docker kubernetes helm argo-cd devsecops security ci-cd
