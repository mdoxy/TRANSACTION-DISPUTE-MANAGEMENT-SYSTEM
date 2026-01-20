# TRANSACTION-DISPUTE-MANAGEMENT-SYSTEM

TRANSACTION DISPUTE MANAGEMENT SYSTEM (TDMS)

Project Overview  
The Transaction Dispute Management System (TDMS) is a secure, full-stack backend application designed to simulate a real-world transaction dispute handling workflow commonly used in payment and financial systems. It allows users to raise disputes for failed or incorrect transactions, while administrators can review, manage, and resolve those disputes through a role-based system.

This project focuses on secure REST API design, backend processing, and role-based access control, making it suitable for enterprise-level applications.

Objectives  
- Build secure and scalable RESTful APIs using Java and Spring Boot  
- Implement JWT-based authentication and authorization  
- Design a role-based system for users and administrators  
- Simulate real-world transaction dispute workflows  
- Follow clean architecture and best coding practices  

System Functionality  

User  
- Register and log in securely  
- Raise a dispute for a transaction  
- View and track dispute status  

Admin  
- View all transaction disputes  
- Review and update dispute status  
- Manage disputes securely using role-based access  

Dispute Workflow  
PENDING → APPROVED → RESOLVED / REJECTED  

System Architecture  
Client (Frontend)  
↓  
Spring Boot REST APIs  
↓  
MySQL Database  

The backend exposes RESTful APIs consumed by a frontend application (ReactJS), while handling authentication, authorization, and business logic internally.

Technology Stack  

Backend  
- Java  
- Spring Boot  
- Spring Security  
- Spring Data JPA  

Security  
- JWT (JSON Web Token)  
- BCrypt Password Encoding  
- Role-Based Access Control  

Database  
- MySQL  

Tools  
- Git & GitHub  
- Postman  
- Maven  

Project Structure  

src/main/java/com/tdms  
 ├── controller     → REST API endpoints  
 ├── service        → Business logic  
 ├── repository     → Database access layer  
 ├── model          → Entity classes  
 ├── dto            → Request/Response objects  
 ├── security       → JWT & security configuration  
 ├── exception      → Global exception handling  
 └── TdmsApplication.java  

API Endpoints Summary  

Authentication  
POST   /api/auth/
