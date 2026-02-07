# Item Management API

A simple Spring Boot REST API for managing items.
This project demonstrates basic CRUD operations using Java, Spring Boot, and Maven.

🚀 Features

Create a new item

Get item by ID

RESTful API design

JSON request & response

Built with Spring Boot and Java 17

🛠️ Tech Stack

Java 17

Spring Boot

Maven

Tomcat (embedded)

REST API

📁 Project Structure
src/main/java
└── com.example.itemapi
    ├── controller
    │   └── ItemController.java
    ├── model
    │   └── Item.java
    ├── service
    │   └── ItemService.java
    └── ItemManagementApiApplication.java

▶️ How to Run the Project
Using Eclipse

Import project as Existing Maven Project

Right-click on ItemManagementApiApplication.java

Select Run As → Java Application

Using Command Line
mvn spring-boot:run


Application will start on:

http://localhost:8080

📌 API Endpoints
➕ Create Item

POST /api/items

{
  "name": "Laptop",
  "description": "Gaming laptop",
  "price": 75000
}

📄 Get Item by ID

GET /api/items/{id}

Example:

GET http://localhost:8080/api/items/1

🧪 Testing with cURL
curl --location 'http://localhost:8080/api/items' \
--header 'Content-Type: application/json' \
--data '{
  "name": "Laptop",
  "description": "Gaming laptop",
  "price": 75000
}'

📦 Build JAR
mvn clean package
