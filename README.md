# Library Management System

A beginner-friendly Java Full Stack Library Management System using **JSP + Servlet + MVC + Service + DAO + JDBC + MySQL + Maven**.

## Architecture

```text
JSP / HTML / CSS
       ↓
Servlet (Controller)
       ↓
Service
       ↓
DAO
       ↓
JDBC
       ↓
MySQL
```

## Features

- Admin login/logout
- Book add/view/delete
- Member add/view
- Issue book
- Return book
- Fine calculation (₹5 per late day)
- JDBC transactions for issue/return
- Maven WAR project

## Project structure

```text
LibraryManagementSystem/
├── README.md
├── .gitignore
├── pom.xml
├── database/schema.sql
└── src/main/
    ├── java/com/library/
    │   ├── model/
    │   ├── dao/
    │   ├── service/
    │   ├── controller/
    │   └── util/
    └── webapp/
        ├── *.jsp
        ├── css/style.css
        └── WEB-INF/web.xml
```

## Run locally

1. Install JDK 17+, Maven, MySQL 8+, and Tomcat 10.1+.
2. Run `database/schema.sql` in MySQL.
3. Open `src/main/java/com/library/util/DBConnection.java` and change the MySQL password.
4. Run `mvn clean package`.
5. Deploy `target/library.war` to Tomcat.
6. Open `http://localhost:8080/library/`.

Demo login: `admin` / `admin123`

> The demo login uses a simple password for learning. Do not use it as-is in production. Use password hashing and authorization filters for a real application.
