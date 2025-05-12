# 🛒 EcomHub

A full-featured e-commerce web application designed for seamless online shopping and admin management.

## 📌 Project Title and Short Description
**EcomHub** - A Spring Boot-based e-commerce backend API supporting key features like user management, product handling, cart functionality, and order processing.

## 🚀 Features
### User Management
- **Register and log in as a user.**
- **User authentication** using JWT (JSON Web Tokens).
- **View and manage user profile** and **addresses**.

### Product Management
- **Add, update, delete**, and **view products**.
- **Search products** by name, category, etc.
- **Display product details** including image, description, and price.

### Order Management
- **Place orders** with the selected products.
- **View and track orders**.
- **Manage order status** and order history.

### Payment Integration
- **Integrate various payment methods** for order completion.
- Handle **payment status and responses** (e.g., success, failure).

### Address Management
- **Add, update, delete**, and **view addresses**.
- **Link addresses** to user accounts for orders.

### Admin Features
- **Manage users, orders, and products**.
- **View sales and product analytics**.

## 🧰 Tech Stack / Technologies Used
- **Language**: Java 17+
- **Backend**: Spring Boot, Spring Security, Spring Data JPA
- **Database**: MySQL
- **Authentication**: JWT (JSON Web Token)
- **Build Tool**: Maven
- **API Testing**: Postman

## 📂 Project Structure
```
ecomhub/
├── src/
│ ├── main/
│ │ ├── java/com/ecommerce/project/
│ │ │ ├── config/
│ │ │ ├── controller/
│ │ │ ├── exceptions/
│ │ │ ├── model/
│ │ │ ├── payload/
│ │ │ ├── repositories/
│ │ │ ├── security/
│ │ │ ├── service/
│ │ │ ├── util/
│ │ │ └── SbEcommerceApplication.java
│ │ ├── resources/
│ │ │ └── application.properties
├── postman/
│ └── ecom_api_collection.json
├── pom.xml
└── README.md
```

## 📦 Installation and Setup Instructions

### Prerequisites
- Java 17 or higher
- MySQL
- Maven

### 1. Clone the Repository
```bash
git clone https://github.com/nikhilsingh2005/ecomhub.git
cd ecomhub
```

### 2. Create the Database
```sql
CREATE DATABASE ecommerce;
```

### 3. Configure MySQL in `application.properties`
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce
spring.datasource.username=yourUsername
spring.datasource.password=yourPassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect
```

### 4. Build and Run
```bash
mvn clean install
mvn spring-boot:run
```

Access the API at: `http://localhost:8080/api/`

## 📬 API Documentation
- Postman collection included in `postman/ecom_api_collection.json`
- Easily import into Postman for testing

## 🤝 Contributing Guidelines
Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## 📧 Contact / Author Info
**Author**: Nikhil Singh  
**GitHub**: [nikhilsingh2005](https://github.com/nikhilsingh2005)