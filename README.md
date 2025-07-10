# 🏥 Patient Management System

A microservices-based healthcare management system built using **Java**, **Spring Boot**, **Kafka**, **Docker**, and **PostgreSQL**. The system handles patient records, billing, analytics, authentication, and secure API communication.

---

## 🧰 Tech Stack

- Java 17+
- Spring Boot 3
- PostgreSQL
- Kafka
- Docker & Docker Compose
- gRPC & REST APIs
- JWT Authentication

---

## 🚀 Microservices Overview

- **auth-service**: User registration & JWT-based authentication
- **patient-service**: CRUD operations for patient data
- **billing-service**: Calculates bills and listens to patient events via Kafka
- **analytics-service**: Consumes Kafka events and tracks system usage
- **api-gateway**: Routes requests and handles security with JWT
- **grpc-requests**: Handles gRPC communication
- **infrastructure**: Contains Docker and environment config

---

## 🛠 How to Run

> All services are containerized using Docker. Kafka, PostgreSQL, and services will start together.

```bash
# Clone the repository
git clone https://github.com/Mahmudul-Hasan-Mukit/Patient_Management_System.git
cd Patient_Management_System

# Run the app
docker-compose up --build
