# PizzaExpress

DESCRIPTION:
-----------
 A full-stack web application that allows customers to place pizza orders, view order history, and check order status. Admins (or the backend) can track order processing using order statuses.
 
TECHNOLOGIES USED:
-----------------
**Backend (Java + Spring Boot) :**

Spring Boot: Used as the main framework to create RESTful controllers, manage application configuration, and handle MVC logic.

Spring Data JPA: For database operations (CRUD) using repositories without writing SQL queries manually.

Hibernate: JPA implementation for ORM (Object-Relational Mapping).

Jakarta Persistence API (JPA): Used for defining entities like OrderItem and Customer.

**Database :**

MySQL: Relational database used to store customer data, order items, and order status.

JPA Repositories: Interfaces like CustomerRepository and OrderItemRepository interact with the MySQL database.

**Frontend :**

HTML/CSS: Used to build the UI for the order form and display pages.

**Other Java Componenets :**

Enums: Used to define OrderStatus (e.g., PENDING, PROCESSING, COMPLETED).

Annotations: @Entity, @Controller, @Repository, @Autowired, etc., to simplify Spring development.

MVC Pattern: Followed to separate concerns between Model (entities), View (HTML pages), and Controller (Spring controller).

**Features Implemented: **
---------------------------

1.Pizza order placement form.

2.Customer and order details stored in MySQL.

3.Paginated order list (/orders endpoint).

4.Order status check by ID (/orderStatus/{id}).

5.Pizza names and prices managed via backend logic.

6.Success page shown after order placement.

** Project Folder Structure**
-----------------------------

pizza-project/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/example/pizza/
│       │       ├── controller/
│       │       │   └── OrderController.java
│       │       ├── entity/
│       │       │   ├── Customer.java
│       │       │   └── OrderItem.java
│       │       ├── enums/
│       │       │   └── OrderStatus.java
│       │       └── repository/
│       │           ├── CustomerRepository.java
│       │           └── OrderItemRepository.java
│       ├── resources/
│       │   ├── application.properties
│       │   └── templates/ (if using Thymeleaf)
│       │       ├── form.html
│       │       ├── orderList.html
│       │       ├── orderStatus.html
│       │       └── success.html
│       │   └── static/
│       │       └── css/
│       │           └── styles.css
├── pom.xml (for Maven dependencies)
└── README.md


## Technologies Used details : 
- Java 17
- Spring Boot
- Spring Data JPA
- MySQL
- HTML/CSS
- MVC Architecture

## Setup
1. Clone the repo
2. Configure `application.properties` with your MySQL credentials
3. Run the application using your IDE or `mvn spring-boot:run`
4. Access `http://localhost:8080/`

## Author

_SAJJARAO RAKESH_ – [https://www.linkedin.com/in/sajjarao-rakesh-837234281/]




