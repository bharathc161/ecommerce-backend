**E-Commerce Project**

**Overview**

This is a Spring Boot-based e-commerce project that provides a backend API for managing products. The project includes features such as product CRUD operations, image handling, and search functionality.

**Technologies Used**

Java
Spring Boot
Spring Data JPA
H2 Database
Lombok
REST API

**Setup Instructions**
Prerequisites
Java 17 or later
Maven

**Any IDE (IntelliJ IDEA, Eclipse, VS Code)

Clone the Repository**

git clone <repository-url>
cd ecom-project

Build and Run the Project

mvn spring-boot:run

**Application Properties**

The application uses an in-memory H2 database. Configuration is as follows:

spring.application.name=ecom-project
spring.datasource.url=jdbc:h2:mem:mydb
spring.datasource.driverClassName=org.h2.Driver
spring.jpa.show-sql=true
spring.jpa.hibernate.ddl-auto=update
spring.jpa.defer-datasource-initialization=true

**API Endpoints

Product Management**

GET /api/products - Retrieve all products

GET /api/product/{id} - Retrieve a product by ID

POST /api/product - Add a new product (with an image)

PUT /api/product/{id} - Update an existing product

DELETE /api/product/{id} - Delete a product

GET /api/product/{productId}/image - Retrieve product image

GET /api/products/search?keyword= - Search for products

**Project Structure**

com.example.ecom_project
│── controller       # Handles API requests
│── model            # Defines data models
│── repo             # Database repository interfaces
│── service          # Business logic and services
│── EcomProjectApplication.java  # Main application entry point

**Dependencies**

Spring Boot Starter Web
Spring Boot Starter Data JPA
H2 Database
Lombok

**Future Enhancements**

Implement user authentication and authorization
Add support for persistent databases like MySQL or PostgreSQL
Improve search functionality with filters
