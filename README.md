# 🎬 BookMyShow Clone – DevOps CI/CD Project  

👨‍💻 **Author:** Ranshi  

---

## 📌 Project Overview  

This project demonstrates an end-to-end DevOps implementation of a BookMyShow Clone application using modern DevOps tools and AWS cloud services.

The application is containerized using Docker, deployed through a Jenkins CI/CD pipeline, pushed to Docker Hub, deployed on AWS EKS (Kubernetes), and monitored using Prometheus and Grafana.

This project follows a real-world production-style deployment approach.

---

## 🏗️ Architecture Overview  

- Source Code Management – GitHub  
- CI/CD – Jenkins  
- Code Quality – SonarQube  
- Security Scanning – Trivy  
- Containerization – Docker  
- Container Registry – Docker Hub  
- Orchestration – AWS EKS  
- Monitoring – Prometheus & Grafana  
- Notifications – Email Integration  

---

## 🚀 Key Features  

✔ Automated CI/CD Pipeline  
✔ SonarQube Code Quality Analysis  
✔ Trivy Security Scanning  
✔ Docker Image Build & Push  
✔ Kubernetes Deployment on AWS EKS  
✔ Email Notifications (Success/Failure)  
✔ Monitoring with Prometheus  
✔ Visualization with Grafana  

---

## 🐳 Part 1 – Docker Based Deployment  

- Launch Ubuntu EC2 Instance  
- Install Jenkins, Docker, and Trivy  
- Configure SonarQube (Docker container)  
- Create Jenkins Pipeline  
- Build & Push Docker Image  
- Deploy Application using Docker  

Access Application:
http://<public-ip>:3000

---

## ☸ Part 2 – Kubernetes Deployment (AWS EKS)  

- Create IAM User with required policies  
- Install AWS CLI, kubectl, eksctl  
- Create EKS Cluster  
- Configure Jenkins with AWS credentials  
- Deploy application using Kubernetes manifests  
- Expose application via Service  

---

## 📊 Monitoring Setup  

### 🔹 Prometheus
- Installed on Monitoring Server  
- Scrapes:
  - Node Exporter metrics
  - Jenkins metrics

### 🔹 Grafana
- Connected with Prometheus Data Source  
- Imported Dashboards:
  - Node Exporter Dashboard
  - Jenkins Performance Dashboard  

Access Grafana:
http://<monitoring-server-ip>:3000

---

## 📧 Email Integration  

- Configured Gmail App Password  
- Email notifications for:
  - Build Success  
  - Build Failure  

---

## 🛠️ Tools & Technologies Used  

- AWS EC2  
- AWS EKS  
- Jenkins  
- Docker  
- Kubernetes  
- SonarQube  
- Trivy  
- Prometheus  
- Grafana  
- NodeJS  

---

## 📂 Pipeline Stages  

1. Clean Workspace  
2. Checkout from Git  
3. SonarQube Analysis  
4. Quality Gate  
5. Install Dependencies  
6. Trivy Scan  
7. Docker Build & Push  
8. Deploy to Docker / EKS  
9. Email Notification  

---

## 🎯 Learning Outcomes  

- Hands-on CI/CD pipeline implementation  
- Secure container image practices  
- Kubernetes deployment in AWS  
- Monitoring and observability setup  
- Production-style DevOps workflow  

---

## 🧹 Cleanup  

After project completion, delete:
- EC2 Instances  
- EKS Cluster  
- IAM Users  
- Security Groups  
- Monitoring Resources  

---

## ⭐ Conclusion  

This project demonstrates a complete DevOps lifecycle implementation from code commit to production deployment and monitoring using industry-standard tools.
