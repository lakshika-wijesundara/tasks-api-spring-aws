# Tasks Management API – Spring Boot (AWS Deployed)

This project is a **RESTful Task Management backend application** built using **Spring Boot** and deployed on **AWS EC2 with Amazon RDS (MySQL)**.  
It demonstrates how a backend application is developed locally and deployed to a real cloud environment.


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
   
**AWS RDS MySQL database instance configuration**
<img width="700" height="853" alt="talinkedin2" src="https://github.com/user-attachments/assets/bfd02a59-0878-4050-9d16-cbd589ff4740" />
MySQL Workbench connection to AWS RDS
**MySQL Workbench connection to AWS RDS**
<img width="700" height="620" alt="talinkedin3" src="https://github.com/user-attachments/assets/47af6e3a-7f30-430c-a195-8be57045de15" />
**AWS EC2 instance summary showing running state and network configuration**
<img width="700" height="891" alt="talinkedin4" src="https://github.com/user-attachments/assets/5affaa9b-83fd-425e-8a5f-405007f12205" />
**Spring Boot application running successfully on EC2 instance**
<img width="700" height="986" alt="talinkedin6" src="https://github.com/user-attachments/assets/6f0ff70e-2e76-4924-bbe6-966e16b7fdb6" />
**Successful user registration API test - POST request returning 200 OK status**
<img width="700" height="915" alt="talinkedin7" src="https://github.com/user-attachments/assets/62c1675a-ae14-476c-8c5c-d2e4e4357e94" />

