# ShopStack 🛒

ShopStack is a Spring Boot REST API backend for managing product categories in an ecommerce system. It demonstrates clean layered architecture using Controller, Service, and Repository layers, along with persistent storage using the H2 in-memory database.

This project serves as a foundation for building scalable ecommerce backend applications using industry-standard backend development practices.

---

## 🚀 Features

* Create new categories
* Retrieve all categories
* Update existing categories
* Delete categories
* Auto-generated unique IDs
* Clean layered architecture
* RESTful API design
* H2 in-memory database integration
* Proper HTTP response handling

---

## 🛠️ Tech Stack

* Java 21
* Spring Boot
* Spring Web
* Spring Data JPA
* H2 Database
* Maven
* REST API

---

## 📁 Project Structure

```
shopstack
│
├── src/main/java/com/ecommerce/project
│   │
│   ├── controller
│   │   └── CategoryController.java
│   │
│   ├── model
│   │   └── Category.java
│   │
│   ├── repositories
│   │   └── CategoryRepository.java
│   │
│   ├── service
│   │   ├── CategoryService.java
│   │   └── CategoryServiceImpl.java
│   │
│   └── ShopstackApplication.java
│
└── pom.xml
```

---

## 🧠 Architecture

This project follows a standard layered backend architecture:

**Controller Layer**

* Handles HTTP requests
* Defines REST endpoints

**Service Layer**

* Contains business logic
* Acts as intermediary between controller and repository

**Repository Layer**

* Handles database operations using Spring Data JPA

**Model Layer**

* Defines database entity structure

---

## ⚙️ Installation and Setup

### Prerequisites

* Java 21 or higher
* Maven
* Git

---

### Clone the repository

```
git clone https://github.com/Aaryamanjhatakia/shopstack.git
cd shopstack
```

---

### Run the application

```
mvn spring-boot:run
```

or

```
mvn clean install
java -jar target/shopstack-0.0.1-SNAPSHOT.jar
```

---

## 📡 API Endpoints

### Create Category

POST `/categories`

Example request body:

```
{
  "name": "Electronics"
}
```

---

### Get All Categories

GET `/categories`

---

### Update Category

PUT `/categories/{id}`

Example request body:

```
{
  "name": "Updated Name"
}
```

---

### Delete Category

DELETE `/categories/{id}`

---

## 🗄️ H2 Database Console

Access at:

```
http://localhost:8080/h2-console
```

Typical configuration:

* JDBC URL: jdbc:h2:mem:testdb
* Username: sa
* Password: (empty)

---

## 🎯 Purpose

This project was built to:

* Learn Spring Boot backend development
* Understand layered architecture
* Practice REST API design
* Work with Spring Data JPA
* Implement database integration

---

## 👨‍💻 Author

Aaryaman Jhatakia

GitHub: [https://github.com/Aaryamanjhatakia](https://github.com/Aaryamanjhatakia)

---


