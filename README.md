<div align="center">

# 🏨 HOTEL MANAGEMENT SYSTEM  
### Desktop Application | Java 11 | JDBC | MySQL

![Java](https://img.shields.io/badge/Java-11-orange)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue)
![JDBC](https://img.shields.io/badge/JDBC-4.2-green)
![Desktop App](https://img.shields.io/badge/Application-Desktop-lightgrey)
![Status](https://img.shields.io/badge/Status-Stable-brightgreen)

</div>

---

## ═══════════════════════════════════════════
## 1. PROJECT OVERVIEW
## ═══════════════════════════════════════════

The **Hotel Management System** is a **Java desktop-based application** designed to automate and manage hotel operations such as:

- Room management  
- Employee management  
- Customer records  
- Driver allocation  

The system is developed using **Java 11**, **JDBC**, and **MySQL**, providing a reliable and scalable solution for small to medium-sized hotels.

---

## ═══════════════════════════════════════════
## 2. PROJECT OBJECTIVES
## ═══════════════════════════════════════════

| Objective | Description |
|---------|-------------|
| Automation | Reduce manual hotel record keeping |
| Accuracy | Improve data consistency |
| Efficiency | Speed up hotel operations |
| Learning | Demonstrate real-world Java development |

---

## ═══════════════════════════════════════════
## 3. SYSTEM FEATURES
## ═══════════════════════════════════════════

| Module | Description |
|------|-------------|
| 🛏 Room Management | Add, update, view hotel rooms |
| 👨‍💼 Employee Management | Manage staff records |
| 🚗 Driver Management | Assign and track drivers |
| 👤 Customer Management | Handle guest information |
| 🔐 Authentication | Secure login system |
| 🖥 Desktop UI | Java Swing-based interface |

---

## ═══════════════════════════════════════════
## 4. SYSTEM ARCHITECTURE
## ═══════════════════════════════════════════

### 4.1 Architectural Pattern

The system follows a **Layered Architecture** with clear separation between:

- Presentation Layer  
- Business Logic Layer  
- Data Access Layer  
- Database Layer  

---

### 4.2 High-Level Architecture Diagram

┌─────────────────────┐
│ User Interface │
│ (Java Swing) │
└──────────┬──────────┘
│
┌──────────▼──────────┐
│ Business Logic Layer│
│ (Controllers) │
└──────────┬──────────┘
│
┌──────────▼──────────┐
│ Data Access Layer │
│ (JDBC / DAO) │
└──────────┬──────────┘
│
┌──────────▼──────────┐
│ MySQL Database │
└─────────────────────┘


---

### 4.3 Layer Responsibility Table

| Layer | Responsibility | Technology |
|-----|----------------|------------|
| Presentation | User interaction | Java Swing |
| Business Logic | System rules | Java |
| Data Access | DB communication | JDBC |
| Database | Data storage | MySQL |

---

## ═══════════════════════════════════════════
## 5. DATABASE DESIGN
## ═══════════════════════════════════════════

### 5.1 Entity Relationship Diagram (Textual)

CUSTOMER ─────┐
ROOM ─────┼── HOTEL DATABASE
EMPLOYEE ─────┤
DRIVER ─────┘


---

### 5.2 Core Tables

| Table | Description |
|------|-------------|
| customer | Stores customer details |
| room | Stores room information |
| employee | Stores staff records |
| driver | Stores driver details |

---

## ═══════════════════════════════════════════
## 6. TECHNOLOGY STACK
## ═══════════════════════════════════════════

| Category | Technology |
|--------|------------|
| Programming Language | Java 11 |
| UI Framework | Java Swing |
| Database | MySQL |
| Data Access | JDBC |
| Build Tool | Apache Ant |
| IDE | NetBeans / IntelliJ |

---

## ═══════════════════════════════════════════
## 7. PROJECT STRUCTURE
## ═══════════════════════════════════════════

Hotel-Management-System/
│
├── src/
│ └── hotel/
│ ├── management/
│ │ ├── HotelManagementSystem.java
│ │ ├── Login.java
│ │ ├── Dashboard.java
│ │ └── modules/
│ └── db/
│ └── DatabaseConnection.java
│
├── nbproject/
├── build.xml
├── manifest.mf
└── README.md


---

## ═══════════════════════════════════════════
## 8. INSTALLATION & SETUP
## ═══════════════════════════════════════════

### 8.1 Prerequisites

- Java JDK 11
- MySQL Server
- NetBeans IDE

---

### 8.2 Installation Steps

1. Clone the repository  
git clone https://github.com/mwakidenis/Hotel-Management-System.git

2. Open project in NetBeans  
3. Import MySQL database (`src/hotel/mysql_command.txt`)  
4. Add required JARs to classpath  
5. Run `HotelManagementSystem.java`

---

## ═══════════════════════════════════════════
## 9. DEFAULT LOGIN CREDENTIALS
## ═══════════════════════════════════════════

| Field | Value |
|-----|------|
| Username | `admin` |
| Password | `12345` |

---

## ═══════════════════════════════════════════
## 10. SCREENSHOTS
## ═══════════════════════════════════════════

| Page | Preview |
|----|---------|
| Landing Page | Screenshot |
| Login Page | Screenshot |
| Dashboard | Screenshot |

---

## ═══════════════════════════════════════════
## 11. CONTRIBUTING
## ═══════════════════════════════════════════

Contributions are welcome.

- Fork the repository  
- Create a feature branch  
- Submit a pull request  

---

## ═══════════════════════════════════════════
## 12. SOURCE & CREDITS
## ═══════════════════════════════════════════

- **Adapted From:**  
*UDEMY – 45 Real World Java Development Projects Bootcamp*

- **Project Author:**  
Engineering.Org.In

- **Last Updated:**  
September 2022

---

<div align="center">

📘 **Professional Academic Documentation**  
✔ Clear Sections  
✔ GitHub Compatible  
✔ University-Ready  

</div>
