# React-Spring CRUD Application

This repository contains a full-stack CRUD application built with **React** for the frontend and **Spring Boot** for the backend. The backend connects to a relational database for data persistence.

## Prerequisites

Before running the application, ensure you have the following installed on your system:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [Java JDK](https://www.oracle.com/java/technologies/javase-downloads.html) (v17 or higher)
- [Maven](https://maven.apache.org/)
- [MySQL](https://www.mysql.com/) or another relational database

---

## Running the Frontend (React)

1. Navigate to the frontend directory:
   ```bash
   cd react-frontend
   ```
## install dependecies 
   ```bash
   npm install
   ```
## start the react developement server  
   ```bash
   npm start 
   ```
## open your browser and navigate to 
```bash
http://localhost:3000
```
## Backend (Spring Boot)

### 1. Navigate to the Backend Directory

To work with the backend, navigate to the backend directory:

```bash
cd springboot-backend
```
### 2. Configure the Database Connection

Before running the backend, you need to configure the database connection. Follow these steps:

1. Open the configuration file:
```bash
src/main/resources/application.properties
```

2. Add the following database configuration:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
spring.datasource.username=your_database_username
spring.datasource.password=your_database_password
spring.jpa.hibernate.ddl-auto=update
```
### 3. Replace the Placeholders with Your Database Credentials

Replace the placeholders in the database configuration with your actual credentials:

- `your_database_name`: The name of your MySQL database. For example, `crud_database`.
- `your_database_username`: Your MySQL username. For example, `root`.
- `your_database_password`: Your MySQL password. For example, `password123`.

### 4. Build the Backend

To build the backend, run the following command in the `springboot-backend` directory:

```bash
mvn clean install
```
### 5. Run the Backend Server

To start the Spring Boot backend server, follow these steps:

1. Open a terminal and navigate to the `springboot-backend` directory:
   ```bash
   cd springboot-backend
```
2.Run the following command to start the server:

mvn spring-boot:run
```
3.Once the server is running, it will be accessible at:
```bash
http://localhost:8080
```
### 6. Database Setup

If the database does not already exist, follow these steps to create it:

1. Open your MySQL terminal or a database client like MySQL Workbench.

2. Run the following SQL command to create the database:
   ```sql
   CREATE DATABASE your_database_name;

