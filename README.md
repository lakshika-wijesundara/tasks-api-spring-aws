# Tasks Management API – Spring Boot (AWS Deployed)

This project is a **RESTful Task Management backend application** built using **Spring Boot** and deployed on **AWS EC2 with Amazon RDS (MySQL)**.  
It demonstrates how a backend application is developed locally and deployed to a real cloud environment.

---

## 🚀 Features
- User Registration & Login (JWT Authentication)
- Create, Update, Delete, and View Tasks
- Task filtering by status and priority
- Secure APIs using Spring Security
- Cloud deployment using AWS EC2 & RDS

---

## 🛠 Tech Stack
- **Backend:** Spring Boot, Spring Security, JWT
- **Database:** MySQL (Amazon RDS)
- **ORM:** JPA / Hibernate
- **Build Tool:** Maven
- **Cloud:** AWS EC2, AWS RDS
- **Testing:** Postman

---

## ☁️ Deployment Architecture
- Spring Boot application runs on **AWS EC2 (Amazon Linux)**
- MySQL database hosted on **Amazon RDS**
- EC2 connects securely to RDS using Security Groups
- APIs accessed publicly using EC2 public IP and custom port

---

## 🔐 Security
- JWT-based authentication
- Protected task APIs (user-specific access)
- Security Groups configured with minimum required ports

---

## 📦 Deployment Steps (Summary)

1. Created MySQL database using **Amazon RDS**
2. Configured database connection in `application.properties`
3. Built the project as an executable JAR
4. Launched **EC2 instance (Amazon Linux)**
5. Configured Security Groups (SSH + Application Port)
6. Copied JAR file to EC2 server
7. Ran the application using:
   ```bash
   java -jar tasksapp.jar
