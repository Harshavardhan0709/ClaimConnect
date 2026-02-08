# ClaimConnect - Insurance Claim Processing System

![Java](https://img.shields.io/badge/Java-17-orange)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.0-green)
![React](https://img.shields.io/badge/React-18-blue)
![Microservices](https://img.shields.io/badge/Architecture-Microservices-red)
![Docker](https://img.shields.io/badge/Docker-Enabled-blue)

## 📌 Overview
**ClaimConnect** is a scalable, microservices-based insurance claim processing system. It streamlines the communication between hospitals, patients, and insurance providers. 
Built with **Spring Boot** for the backend and **React** for the frontend, it ensures modularity, security, and high availability.

## 🏗 Architecture
The system follows a distributed microservices architecture:

* **API Gateway:** Secure entry point for all client requests.
* **Eureka Server:** Service discovery for dynamic scaling.
* **Config Server:** Centralized configuration management via GitHub.
* **Microservices:** Decoupled services for Claims, Hospitals, Patients, and Insurance logic.

## 🚀 Key Features
* ✅ **Microservices Architecture:** Independently deployable and scalable services.
* ✅ **Service Discovery:** Automated service registration using **Netflix Eureka**.
* ✅ **Centralized Config:** Configurations managed externally via **Spring Cloud Config**.
* ✅ **API Gateway:** Centralized routing and load balancing using **Spring Cloud Gateway**.
* ✅ **Security:** JWT Authentication and Role-Based Access Control (RBAC).
* ✅ **Inter-service Communication:** RESTful APIs with **Feign Clients**.
* ✅ **Frontend:** Responsive UI built with **React** and **Bootstrap**.

## 🛠 Tech Stack

### Backend
* **Language:** Java 17
* **Framework:** Spring Boot, Spring Cloud (Gateway, Eureka, Config)
* **Database:** MySQL
* **Build Tool:** Maven

### Frontend
* **Library:** React.js
* **State Management:** Redux
* **Styling:** Bootstrap CSS

### DevOps & Tools
* **Containerization:** Docker
* **Orchestration:** Kubernetes (K8s)
* **Version Control:** Git & GitHub

## 📂 Microservices Breakdown
1.  **Config Server:** Manages external properties for all services.
2.  **Eureka Server:** Registry for all microservices.
3.  **API Gateway:** Routes traffic to specific services.
4.  **Patient Service:** Manages patient demographics and history.
5.  **Hospital Service:** Handles hospital records and doctor details.
6.  **Claim Service:** Core logic for submitting and processing claims.
7.  **Insurance Service:** Validates policies and approves settlements.

## ⚙️ Getting Started

### Prerequisites
* Java 17+
* Node.js & npm
* MySQL Server
* Docker (Optional)

### Installation Steps

1.  **Clone the Repository**
    bash
    git clone [https://github.com/Harshavardhan0709/ClaimProcessingSystem.git](https://github.com/Harshavardhan0709/ClaimProcessingSystem.git)
    cd ClaimProcessingSystem
    

2.  **Database Setup**
    * Create a MySQL database named "claim_db".
    * Update "application.properties" in the Config Server repo with your DB credentials.

3.  **Run Microservices (Order Matters)**
    * Start **Config Server**
    * Start **Eureka Server**
    * Start **API Gateway**
    * Start **Patient / Hospital / Claim Services**

4.  **Run Frontend**
    bash
    cd frontend
    npm install
    npm start
    

## 🐳 Docker Support
To run the entire system using Docker Compose:
bash
docker-compose up -d
