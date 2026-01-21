<div align="center">

# 👤 USER MANAGEMENT SYSTEM  
### JSP • Servlet • JDBC • MySQL CRUD Application

![Java](https://img.shields.io/badge/Java-JDK%208+-orange)
![JSP](https://img.shields.io/badge/JSP-2.2-blue)
![Servlet](https://img.shields.io/badge/Servlet-2.5-green)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue)
![Tomcat](https://img.shields.io/badge/Tomcat-8.5-yellow)
![MVC](https://img.shields.io/badge/Architecture-MVC-brightgreen)

📘 **Academic-grade Java Web Application**  
📦 **CRUD | MVC | DAO | JDBC | Tomcat Deployment**

</div>

---

## 📌 Project Overview

The **User Management System** is a Java EE web application developed using **JSP, Servlets, JDBC, and MySQL**.  
It demonstrates **full CRUD functionality (Create, Read, Update, Delete)** while strictly following the  
**MVC (Model–View–Controller)** architectural pattern.

This project is suitable for:
- 🎓 University assignments  
- 💼 Java Web portfolios  
- 🧪 Learning JDBC & MVC  
- 🚀 Tomcat-based deployments  

---

## ✨ Core Features

| Feature | Description |
|---|---|
| ➕ Create User | Add new users to the system |
| 📋 View Users | Display all users in a table |
| ✏️ Update User | Edit existing user details |
| ❌ Delete User | Remove a user from database |
| 🧱 MVC Pattern | Clean separation of concerns |
| 🗃 DAO Pattern | Centralized DB access |
| 🎨 UI Styling | Bootstrap 4 |

---

## 🏗 System Architecture (MVC)

### High-Level Flow

Browser
│
▼
JSP Views (UI / Forms)
│
▼
Servlet Controller (UserServlet)
│
▼
DAO Layer (UserDAO)
│
▼
MySQL Database (users)


### MVC Responsibility Mapping

| Layer | Responsibility | Technology | Files |
|---|---|---|---|
| View | UI rendering | JSP, JSTL, Bootstrap | user-list.jsp, user-form.jsp |
| Controller | Request handling | Servlet API | UserServlet.java |
| Model | Data structure | JavaBean | User.java |
| DAO | Database logic | JDBC | UserDAO.java |
| Database | Persistent storage | MySQL | users table |

---

## 🗄 Database Design (ERD)

### Entity Structure

USERS
id INT (PK)
name VARCHAR
email VARCHAR
country VARCHAR


**Notes**
- Single-entity system
- `id` is AUTO_INCREMENT
- Designed for basic CRUD operations

---

## 🛠 Technology Stack

| Category | Technology |
|---|---|
| Language | Java (JDK 8+) |
| Frontend | JSP 2.2, JSTL 1.2.1 |
| Backend | Servlet API 2.5 |
| Database | MySQL |
| Data Access | JDBC 4.2 |
| Server | Apache Tomcat 8.5 |
| UI | Bootstrap 4 |
| IDE | Eclipse / STS |

---

## 📁 Project Structure

jsp-servlet-jdbc-mysql-example/
│
├── src/
│ └── net/javaguides/usermanagement/
│ ├── model/
│ │ └── User.java
│ ├── dao/
│ │ └── UserDAO.java
│ └── web/
│ └── UserServlet.java
│
├── WebContent/
│ ├── user-list.jsp
│ ├── user-form.jsp
│ ├── error.jsp
│ └── index.jsp
│
└── README.md


---

## 🗃 Database Setup

### Create Database
```sql
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
🔄 Application Request Flow
Step	Action
1	User sends request from browser
2	JSP submits form
3	Servlet processes request
4	DAO executes SQL
5	MySQL returns result
6	Servlet forwards response
7	JSP renders output
🌐 URL Mapping
URL Pattern	Function
/list	Display users
/new	Show add form
/insert	Insert user
/edit	Edit user
/update	Update user
/delete	Delete user
🚀 Deployment Steps
Prerequisites
Java JDK 8+

MySQL Server

Apache Tomcat 8.5

Run Application
Start MySQL server

Start Tomcat

Copy project to:

apache-tomcat-8.5/webapps/
Open browser:

http://localhost:8080/jsp-servlet-jdbc-mysql-example/
<div align="center">
