```markdown
# Product Management System

A Full Stack Java project for managing products, developed using Spring Boot for the backend, React for the frontend, and MySQL as the database.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Features](#features)
- [API Endpoints](#api-endpoints)
- [Frontend Setup](#frontend-setup)
- [Backend Setup](#backend-setup)
- [Database Setup](#database-setup)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project is a Product Management System that allows users to:
- Add, edit, delete, and view products.
- Manage product categories.
- Perform CRUD (Create, Read, Update, Delete) operations on products.
- View product details and inventory.

It uses **Spring Boot** to create RESTful APIs for the backend and **React** for a dynamic and responsive user interface. The backend communicates with a **MySQL** database to store product information.

## Technologies Used

- **Backend**: 
  - Spring Boot
  - Spring Data JPA
  - MySQL
  - REST APIs
  - Hibernate
- **Frontend**:
  - React.js
  - Axios (for API requests)
  - Bootstrap (for UI)
- **Database**: 
  - MySQL
  
## Installation

### Backend Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/AbishekMJ/product-management-system.git
   ```

2. Navigate to the backend directory:
   ```bash
   cd product-management-system/backend
   ```

3. Install dependencies:
   - For Spring Boot, you can use Maven or Gradle. Make sure to have JDK 11 or higher installed.
   - You can also import the project into your IDE (e.g., IntelliJ IDEA, Eclipse).

4. Set up MySQL database:
   - Create a database named `product_management_db`.
   - Modify `application.properties` (located in `src/main/resources/application.properties`) with your database credentials:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/product_management_db
     spring.datasource.username=root
     spring.datasource.password=password
     ```

5. Run the Spring Boot application:
   ```bash
   ./mvnw spring-boot:run
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd product-management-system/frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the React application:
   ```bash
   npm start
   ```

4. Open your browser and go to `http://localhost:3000` to access the frontend.

## Features

- **User Authentication**: Login/Logout functionality (can be extended with JWT token authentication).
- **Product Management**: 
  - Add, Edit, and Delete products.
  - Display product details.
  - Manage product categories.
- **Search Functionality**: Search products by name or category.
- **Responsive UI**: Optimized for mobile and desktop.

## API Endpoints

### Product APIs

- **GET** `/api/products`: Get all products.
- **GET** `/api/products/{id}`: Get product by ID.
- **POST** `/api/products`: Add a new product.
- **PUT** `/api/products/{id}`: Update an existing product.
- **DELETE** `/api/products/{id}`: Delete a product.

### Category APIs

- **GET** `/api/categories`: Get all product categories.
- **POST** `/api/categories`: Add a new category.
  
## Frontend Setup

The frontend is built with React.js and Axios for HTTP requests.

1. To run the frontend, navigate to the frontend directory and run:
   ```bash
   npm start
   ```

2. The frontend makes HTTP requests to the backend, so ensure the backend is running first.

## Backend Setup

1. The backend is a Spring Boot application.
2. The backend exposes REST APIs to interact with product and category data.
3. Use MySQL to store product and category data.

## Database Setup

1. Set up a MySQL database with the following schema:
   ```sql
   CREATE DATABASE product_management_db;
   ```

2. You can use the provided `schema.sql` file to create necessary tables.

## Contributing

Feel free to fork the repository, create branches, and submit pull requests. Any improvements, bug fixes, or new features are highly appreciated!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

This template includes sections for setting up both the backend and frontend, listing the technologies used, and providing API endpoints for the application. You can adjust the database configurations and other specifics based on your project structure.
