
# Student Management System

A backend REST API project developed using Java, Spring Boot, Spring Data JPA, Hibernate, and MySQL. This application provides CRUD (Create, Read, Update, Delete) operations to manage student records efficiently.

## 🚀 Technologies Used

- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- MySQL
- Maven
- REST API
- Postman
- IntelliJ IDEA

## ✨ Features

- Add a new student
- Retrieve all students
- Retrieve student by ID
- Update student details
- Delete student by ID
- Store student information in MySQL database
- Exception handling for student records

## 📂 Project Structure

```text
StudentManagementSystem
│
├── src/main/java/com/papai/studentmanagement
│   ├── controller
│   │   └── StudentController.java
│   ├── service
│   │   └── StudentService.java
│   ├── repository
│   │   └── StudentRepository.java
│   ├── entity
│   │   └── Student.java
│   ├── exception
│   │   └── StudentNotFoundException.java
│   └── StudentManagementApplication.java
│
├── src/main/resources
│   └── application.properties
│
├── pom.xml
└── README.md
```

## ⚙️ Database Configuration

Create a MySQL database:

```sql
CREATE DATABASE student_management;
```

Configure `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/student_management
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

## 🔗 REST API Endpoints

Base URL:

```text
http://localhost:8080/api/students
```

| HTTP Method | Endpoint | Description |
|---|---|---|
| POST | `/api/students` | Add a new student |
| GET | `/api/students` | Get all students |
| GET | `/api/students/{id}` | Get student by ID |
| PUT | `/api/students/{id}` | Update student |
| DELETE | `/api/students/{id}` | Delete student |

## 📥 Sample JSON Request

Add Student:

```json
{
  "name": "Rahul Sharma",
  "email": "rahul@gmail.com",
  "department": "Computer Science",
  "age": 21
}
```

## 🛠️ How to Run the Project

1. Clone the repository.
2. Open the project in IntelliJ IDEA.
3. Configure MySQL database credentials in `application.properties`.
4. Make sure MySQL server is running.
5. Update Maven dependencies.
6. Run `StudentManagementApplication.java`.
7. Test REST API endpoints using Postman.

## 🎯 Learning Outcomes

- Understanding Spring Boot application architecture.
- Implementing RESTful web services.
- Working with Spring Data JPA and Hibernate.
- Performing CRUD operations using JpaRepository.
- Connecting Spring Boot with MySQL.
- Understanding Controller, Service, and Repository layers.

## 👨‍💻 Author

**Papai Samui**

---
⭐ If you find this project useful, consider giving it a star!
