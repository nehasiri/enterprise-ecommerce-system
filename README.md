# Full Stack E-commerce Platform

A full-stack e-commerce application built using **Spring Boot (Java)** for the backend and **React with Vite** for the frontend. The application demonstrates real-world full-stack development practices, including RESTful API design, frontend–backend integration, and relational database persistence.

---

## 📁 Project Structure

```text
springboot-react-ecommerce-platform/
├── ecommerce-api/     # Spring Boot REST API backend
├── ecommerce-ui/      # React + Vite frontend application
```

## 🧩 Backend – Spring Boot (`ecommerce-api`)

## 📁 Project Structure

### 🔧 Technologies Used
- Java 8+
- Spring Boot
- Spring Data JPA
- Hibernate
- RESTful APIs
- MySQL
- Maven

### 📂 Backend Directory Structure
``` text
ecommerce-api/
├── controller/        # REST API controllers
├── service/           # Business logic layer
├── repository/        # Spring Data JPA repositories
├── model/             # JPA entity classes
├── config/            # Application configuration
├── resources/
│   ├── application.properties
│   └── data.sql       # Initial seed data
└── pom.xml            # Maven configuration
```
### ⚙️ Backend Setup Instructions
**Database Configuration**

Create a MySQL database:

```text
ecomdb
```


Update `application.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/ecomdb
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
```

Run the Backend
```bash
cd ecommerce-api
mvn spring-boot:run
```


Initial product data is loaded automatically on first run using data.sql.

---

### 📡 REST API Endpoints
| Method | Endpoint | Description |
|------|---------|-------------|
| GET | /products | Fetch all products |
| GET | /products/{id} | Fetch product by ID |
| POST | /products | Create new product |
| PUT | /products/{id} | Update product |
| DELETE | /products/{id} | Delete product |

---

## 💻 Frontend – React + Vite (`ecommerce-ui`)

### 🔧 Technologies Used
- React
- Vite
- JavaScript (ES6+)
- Axios
- Bootstrap
- HTML5
- CSS3

### 📂 Frontend Directory Structure
```text
ecommerce-ui/
├── public/
├── src/
│   ├── components/    # Reusable UI components
│   ├── pages/         # Page-level views
│   ├── services/      # API integration layer
│   ├── App.jsx        # Application layout
│   └── main.jsx       # Entry point
├── package.json
└── vite.config.js
```

### ▶️ Frontend Setup Instructions

Install dependencies:
```bash
cd ecommerce-ui
npm install
```


Run the application:
```bash
npm run dev
```

Frontend will be available at:
```text
http://localhost:5173
```

Ensure backend APIs are reachable:
```text
http://localhost:8080/products
```
## 🧩 Features
- Product listing and management
- RESTful API integration
- Dynamic UI rendering with React
- Responsive frontend design
- Modular backend architecture
- Easily extendable for cart, checkout, authentication, and payment features

## 🚀 Future Enhancements
- User authentication and authorization (JWT)
- Shopping cart and checkout flow
- Order management
- Cloud deployment on AWS
- CI/CD pipeline integration
- Microservices architecture extension


### 📌 Summary

This project showcases end-to-end full-stack development using Java and modern frontend technologies, following clean architecture principles and scalable design practices. It serves as a strong foundation for enterprise-grade e-commerce systems and cloud-ready applications.

### 🔖 Topics
```text
Java SpringBoot React full-stack rest-api ecommerce mysql docker aws
```
