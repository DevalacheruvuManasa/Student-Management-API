# Student Management API

## 📌 Overview
The **Student Management API** is a RESTful web service built with **Spring Boot** and **MySQL** that enables efficient management of student records. It provides CRUD operations to add, update, retrieve, and delete student information with proper validation and testing using **Postman**.

## 🚀 Features
- **Student CRUD Operations**: Create, Read, Update, and Delete students.
- **Spring Boot & MySQL Integration**: Stores and retrieves data securely.
- **Validation & Error Handling**: Ensures data integrity with validation.
- **RESTful API**: Exposes endpoints for seamless integration.
- **Postman Testing**: Verify API responses with Postman.

## 🛠️ Tech Stack
- **Backend**: Java, Spring Boot, Spring Data JPA
- **Database**: MySQL
- **Tools**: Postman, Git, GitHub

## 📂 Project Structure
```
Student-Management-API/
│── src/main/java/com/example/studentmanagement
│   ├── controller/  # API Controllers
│   ├── service/     # Business Logic
│   ├── repository/  # Data Layer
│   ├── entity/      # Entity Classes
│   ├── exception/   # Custom Exceptions
│── src/main/resources/
│   ├── application.properties  # DB Config
│── pom.xml  # Dependencies
│── README.md  # Documentation
```

## 🔗 API Endpoints
| Method | Endpoint           | Description |
|--------|-------------------|-------------|
| GET    | `/students`       | Get all students |
| GET    | `/students/{id}`  | Get student by ID |
| POST   | `/students`       | Add a new student |
| PUT    | `/students/{id}`  | Update student details |
| DELETE | `/students/{id}`  | Delete a student |

## 🏗️ Setup & Installation
### Prerequisites
- Java 11+
- MySQL Database
- Maven
- Postman (for testing API)

### Steps
1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/Student-Management-API.git
   cd Student-Management-API
   ```
2. **Configure MySQL in `application.properties`:**
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/student_db
   spring.datasource.username=root
   spring.datasource.password=manasa05
   spring.jpa.hibernate.ddl-auto=update
   ```
3. **Build and run the application:**
   ```sh
   mvn spring-boot:run
   ```
4. **Test API with Postman or browser:**
   - Open `http://localhost:8080/students`

## 📜 License
This project is open-source and available under the [MIT License](LICENSE).
