# Employee Management System

A modern, full-stack Employee Management System built with Angular (frontend) and Spring Boot (backend).

## Project Overview
- **Frontend:** Angular 10, Bootstrap 4
- **Backend:** Spring Boot 3, MySQL
- **Features:**
  - List all employees
  - Add a new employee
  - Update employee details
  - View employee details
  - Delete an employee

## Project Structure
```
Java_Full_Stack_Proj/
├── angular-frontend/      # Angular 10 application
└── springboot-backend/    # Spring Boot REST API
```

## Frontend (Angular)
- **Directory:** `angular-frontend/`
- **Main routes:**
  - `/employees` — Employee list
  - `/create-employee` — Add new employee
  - `/update-employee/:id` — Update employee
  - `/employee-details/:id` — View employee details
- **Development server:**
  1. Install dependencies: `npm install`
  2. Start: `ng serve`
  3. Open: [http://localhost:4200/](http://localhost:4200/)

## Backend (Spring Boot)
- **Directory:** `springboot-backend/`
- **REST Endpoints:** (all under `/api/v1/`)
  - `GET    /employees` — List all employees
  - `POST   /employees` — Add new employee
  - `GET    /employees/{id}` — Get employee by ID
  - `PUT    /employees/{id}` — Update employee
  - `DELETE /employees/{id}` — Delete employee
- **Database:** MySQL
  - Configure connection in `springboot-backend/src/main/resources/application.properties`
  - Example:
    ```
    spring.datasource.url=jdbc:mysql://localhost:3306/employee_management_system?useSSL=false
    spring.datasource.username=YOUR_DB_USER
    spring.datasource.password=YOUR_DB_PASSWORD
    spring.jpa.hibernate.ddl-auto=update
    ```
- **Run backend:**
  1. Ensure MySQL is running and database is created
  2. Update DB credentials in `application.properties`
  3. In `springboot-backend/`, run: `mvn spring-boot:run`

## Requirements
- Node.js & npm
- Angular CLI
- Java 17+
- Maven
- MySQL

## Credits
All Rights Reserved © Sujit Bhalekar

