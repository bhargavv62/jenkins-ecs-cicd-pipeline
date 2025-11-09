# 🧩 Spring PetClinic CI/CD Pipeline Project

This project is a customized version of the **Spring PetClinic** application, designed to demonstrate a complete **DevOps CI/CD pipeline** on **AWS** using modern tools and automation.

## 🚀 Tools & Technologies
- **Version Control:** Git & GitHub  
- **CI/CD:** Jenkins  
- **Containerization:** Docker  
- **Artifact Management:** JFrog Artifactory  
- **Configuration Management:** Ansible  
- **Infrastructure Provisioning:** Terraform  
- **Orchestration:** Kubernetes (EKS)  
- **Monitoring:** Prometheus & Grafana  
- **Code Quality:** SonarQube  

## 🧱 Pipeline Flow
1. Developer pushes code to GitHub  
2. Jenkins triggers CI pipeline:
   - Code checkout → Build → Unit Test → SonarQube analysis  
   - Docker image build → Push to JFrog Artifactory  
3. CD pipeline provisions AWS infrastructure with Terraform  
4. Ansible deploys application on EKS cluster  
5. Prometheus & Grafana monitor application metrics  

## 🧰 How to Run Locally
```bash
git clone https://github.com/bhargavv62/jenkins-ecs-cicd-pipeline.git
cd spring-petclinic
./mvnw spring-boot:run
