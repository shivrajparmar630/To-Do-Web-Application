# 📝 To-Do Web Application

A web-based **To-Do application** built using **Java, Spring Boot, Spring Data JPA, MySQL, HTML, CSS, and JavaScript**.

The application provides a simple interface to manage daily tasks with **Create, Read, Update, and Delete (CRUD)** functionality.

---

## 🚀 Features

- ✅ Create new tasks
- 📋 View all tasks
- ✏️ Update existing tasks
- 🗑️ Delete tasks
- 💾 Persistent data storage using MySQL
- 🧩 Spring Data JPA for database interaction
- 🔗 RESTful backend architecture
- 🏗️ Layered architecture
- 🎨 Clean and responsive user interface
- 🧪 Spring Boot test support

---

## 🛠️ Tech Stack

### Backend
- Java
- Spring Boot
- Spring MVC
- Spring Data JPA
- Hibernate

### Frontend
- HTML5
- CSS3
- JavaScript

### Database
- MySQL

### Build & Tools
- Maven
- Git
- GitHub
- IntelliJ IDEA

---

## 🏗️ Project Architecture

The application follows a layered architecture:

```text
             Client
                │
                ▼
           Controller
                │
                ▼
             Service
                │
                ▼
           Repository
                │
                ▼
          MySQL Database
```

### Architecture Layers

**Controller**
- Handles incoming HTTP requests
- Communicates with the service layer

**Service**
- Contains application business logic
- Connects the controller and repository layers

**Repository**
- Uses Spring Data JPA
- Handles database operations

**Model**
- Represents the application's data/entity structure

---

## 📂 Project Structure

```text
To-Do-Web-Application/
│
├── .mvn/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/app/todoapp/
│   │   │       ├── controller/
│   │   │       │   └── TaskController.java
│   │   │       │
│   │   │       ├── models/
│   │   │       │   └── Task.java
│   │   │       │
│   │   │       ├── repository/
│   │   │       │   └── TaskRepository.java
│   │   │       │
│   │   │       ├── services/
│   │   │       │   └── TaskService.java
│   │   │       │
│   │   │       └── TodoappApplication.java
│   │   │
│   │   └── resources/
│   │       ├── templates/
│   │       │   └── tasks.html
│   │       │
│   │       └── application.properties
│   │
│   └── test/
│
├── pom.xml
├── mvnw
├── mvnw.cmd
├── .gitignore
├── .gitattributes
└── README.md
```

---

## ⚙️ Prerequisites

Make sure the following are installed:

- Java 17 or later
- MySQL
- Git
- Maven *(optional, Maven Wrapper is included)*

---

## 🗄️ Database Setup

Create a MySQL database:

```sql
CREATE DATABASE todoapp;
```

Then configure your MySQL connection in:

```text
src/main/resources/application.properties
```

Example:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/todoapp
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
```

> Replace `YOUR_PASSWORD` with your local MySQL password.

⚠️ **Do not upload your real database password to GitHub.**

---

## ▶️ Run the Application

### 1. Clone the repository

```bash
git clone https://github.com/shivrajparmar630/To-Do-Web-Application.git
```

### 2. Navigate to the project

```bash
cd To-Do-Web-Application
```

### 3. Run the application

On Windows:

```bash
mvnw.cmd spring-boot:run
```

Or, if Maven is installed:

```bash
mvn spring-boot:run
```

---

## 🌐 Access the Application

Once the application starts successfully, open:

```text
http://localhost:8080
```

---

## 🧪 Testing

Run the test suite using:

```bash
mvn test
```

Or on Windows:

```bash
mvnw.cmd test
```

---

## 🔮 Future Improvements

- 🔐 User authentication and authorization
- 👤 Multiple user support
- ⭐ Task priority
- 📅 Task deadlines
- 🔎 Search and filtering
- 📊 Dashboard and task statistics
- ☁️ AWS deployment
- 🐳 Docker support
- 📱 Improved mobile responsiveness

---

## 👨‍💻 Author

### Shivraj Singh

**Java | Spring Boot | MySQL | JavaScript | SQL**

---

## 📄 License

This project is developed for **learning and educational purposes**.
