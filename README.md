<div align="center">

# 👤 JSP Servlet JDBC MySQL CRUD Application  
### User Management System

<img src="https://img.shields.io/badge/Java-JDK%208+-orange?style=for-the-badge&logo=java"/>
<img src="https://img.shields.io/badge/JSP-Servlets-blue?style=for-the-badge&logo=apachetomcat"/>
<img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql"/>
<img src="https://img.shields.io/badge/Tomcat-8.5-yellow?style=for-the-badge&logo=apachetomcat"/>

<br/>

**A complete CRUD-based Java Web Application using JSP, Servlets, JDBC & MySQL**

</div>

---

## 📌 Project Overview

The **User Management System** is a Java EE web application that demonstrates **Create, Read, Update, and Delete (CRUD)** operations using:

- **JSP** for presentation  
- **Servlets** for request handling  
- **JDBC** for database interaction  
- **MySQL** for persistent data storage  

This project strictly follows the **MVC (Model–View–Controller)** architectural pattern and is deployed on **Apache Tomcat 8.5**.

---

## ✨ Features

- ➕ Create a new user  
- 📋 View all users  
- ✏️ Update user details  
- ❌ Delete a user  
- 🧱 MVC architecture  
- 🗃 DAO design pattern  
- 🎨 Bootstrap-based UI  

---

## 🏗 System Architecture (MVC)

```mermaid
flowchart LR
    A[Browser] --> B[JSP Pages]
    B --> C[UserServlet]
    C --> D[UserDAO]
    D --> E[(MySQL Database)]
Architecture Mapping
Layer	Component
Model	User.java
View	user-list.jsp, user-form.jsp
Controller	UserServlet.java
Data Access	UserDAO.java
🧩 Entity Relationship Diagram (ERD)
erDiagram
    USERS {
        INT id PK
        VARCHAR name
        VARCHAR email
        VARCHAR country
    }
ERD Explanation
Single entity: USERS

id is the Primary Key

Each row represents one user

No foreign key relationships (single-table CRUD system)

🛠 Technology Stack
Layer	Technology
Language	Java (JDK 8+)
Frontend	JSP 2.2, JSTL 1.2.1
Backend	Servlet API 2.5
Database	MySQL
Data Access	JDBC 4.2
Server	Apache Tomcat 8.5
UI	Bootstrap 4
IDE	Eclipse / STS
📁 Project Structure
jsp-servlet-jdbc-mysql-example/
│
├── src/
│   └── net/javaguides/usermanagement/
│       ├── dao/
│       │   └── UserDAO.java
│       ├── model/
│       │   └── User.java
│       └── web/
│           └── UserServlet.java
│
├── WebContent/
│   ├── user-list.jsp
│   ├── user-form.jsp
│   ├── error.jsp
│   └── index.jsp
│
└── README.md
🗄 Database Setup
Create Database
CREATE DATABASE demo;
USE demo;
Create Table
CREATE TABLE users (
  id INT(3) NOT NULL AUTO_INCREMENT,
  name VARCHAR(120) NOT NULL,
  email VARCHAR(220) NOT NULL,
  country VARCHAR(120),
  PRIMARY KEY (id)
);
🔄 Application Flow
sequenceDiagram
    participant U as User
    participant J as JSP
    participant S as Servlet
    participant D as DAO
    participant M as MySQL

    U->>J: Submit Request
    J->>S: HTTP Request
    S->>D: Call CRUD Method
    D->>M: Execute SQL
    M-->>D: Result
    D-->>S: Data
    S-->>J: Forward Response
🚀 Deployment & Execution
Prerequisites
Java JDK 8 or later

MySQL Server

Apache Tomcat 8.5

Steps
Start MySQL Server

Start Apache Tomcat

Copy project folder to:

apache-tomcat-8.5/webapps/
Open browser and visit:

http://localhost:8080/jsp-servlet-jdbc-mysql-example/
🖥 Application Pages
Page	Purpose
user-list.jsp	Displays all users
user-form.jsp	Add / Edit user
error.jsp	Displays runtime errors
⚠ Error Handling
SQL exceptions handled via printSQLException()

Centralized error display using error.jsp

Safe redirects after CRUD actions
