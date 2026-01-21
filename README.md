# 🏨 JSP Servlet JDBC MySQL CRUD Application

A **comprehensive Java web application** that demonstrates how to build a full **CRUD (Create, Read, Update, Delete)** system using **JSP, Servlets, JDBC, and MySQL**, deployed on **Apache Tomcat**.

This project is ideal for **students, beginners, and backend learners** who want to understand how traditional **Java EE web applications** work end-to-end.

---

## 📌 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [System Architecture](#system-architecture)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation & Setup](#installation--setup)
- [Database Setup](#database-setup)
- [Running the Application](#running-the-application)
- [Usage Guide](#usage-guide)
- [Common Errors & Fixes](#common-errors--fixes)
- [Learning Outcomes](#learning-outcomes)
- [Contributing](#contributing)
- [Credits](#credits)

---

## 📖 Overview

This project is a **JSP + Servlet + JDBC + MySQL** based web application that allows users to:

- Add new users
- View a list of users
- Update existing users
- Delete users

The application follows the **MVC (Model–View–Controller)** architecture and runs on **Apache Tomcat**.

> ⚠️ This is **NOT** a React or Node.js application.  
> It runs on a **Java server (Tomcat)** and uses **MySQL** as the database.

---

## ✨ Features

- User CRUD operations
- JSP-based UI
- Servlet controller logic
- JDBC database connectivity
- MySQL integration
- MVC architecture
- Beginner-friendly and well-structured

---

## 🧠 System Architecture

Browser (Chrome)
↓
Apache Tomcat Server (localhost:8080)
↓
Servlet Controller (UserServlet.java)
↓
DAO Layer (UserDAO.java)
↓
MySQL Database (users table)


- **JSP** → View layer (UI)
- **Servlets** → Controller layer
- **DAO** → Database logic
- **MySQL** → Persistent storage

---

## 🛠 Tech Stack

| Technology | Purpose |
|---------|--------|
| Java (8+) | Backend logic |
| JSP | Frontend UI |
| Servlets | Request handling |
| JDBC | Database connectivity |
| MySQL | Database |
| Apache Tomcat 8.5 | Web server |
| Git & GitHub | Version control |

---

## 📁 Project Structure

jsp-servlet-jdbc-mysql-example/
│
├── src/
│ ├── com.example.dao/
│ │ └── UserDAO.java
│ ├── com.example.model/
│ │ └── User.java
│ └── com.example.web/
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

## ⚙️ Installation & Setup

### Prerequisites
Ensure the following are installed:

- Java JDK 8 or higher
- MySQL Server
- Apache Tomcat 8.5
- Git (optional)

---

## 🗄 Database Setup

1. Start MySQL Server
2. Open MySQL client
3. Run the following SQL commands:

```sql
CREATE DATABASE demo;
USE demo;

CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(120),
  email VARCHAR(220),
  country VARCHAR(120)
);
Update database credentials in UserDAO.java if necessary:

private String jdbcUsername = "root";
private String jdbcPassword = "root";
▶️ Running the Application
Step 1: Start Apache Tomcat
Navigate to:

apache-tomcat-8.5.xx/bin
Run:

startup.bat (Windows)

startup.sh (Linux/Mac)

Step 2: Deploy the Project
Copy the project folder:

jsp-servlet-jdbc-mysql-example
Paste it into:

apache-tomcat-8.5.xx/webapps/
Step 3: Open in Browser
http://localhost:8080/jsp-servlet-jdbc-mysql-example/
🎉 Application is now running!

🧪 Usage Guide
Open the app in browser

View all users

Click Add User to create a new record

Edit user details

Delete users as needed

❗ Common Errors & Fixes
❌ 404 Not Found
Tomcat not running

Project not inside webapps

❌ Database Connection Error
MySQL server not running

Incorrect username/password

Database not created

❌ Changes not reflecting
Restart Tomcat after changes

🎓 Learning Outcomes
By working on this project, you will learn:

How JSP & Servlets work together

MVC architecture in Java web apps

JDBC database integration

Deploying apps on Tomcat

Real-world Java backend workflow

🤝 Contributing
Contributions are welcome!

Fork the repository

Create a feature branch

Commit your changes

Open a Pull Request

📚 Credits
Adapted from Java Web Development tutorials and educational resources.

Originally inspired by:
Java Programming Course – JSP, JDBC, Servlets

⭐ If you find this project helpful
Please give it a star ⭐
