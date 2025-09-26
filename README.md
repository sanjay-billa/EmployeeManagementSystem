# Employee Management System

This is a simple Employee Management System built with Java Spring Boot. It provides RESTful APIs to manage employee records, allowing users to create, read, update, and delete employee information. The application uses an in-memory H2 database for persistence, making it easy to test and deploy without external dependencies.

## Features

- **Add Employee:** Create new employee records with name, department, and salary.
- **View Employees:** Retrieve a list of all employees or view details for a specific employee.
- **Update Employee:** Edit employee details by ID.
- **Delete Employee:** Remove an employee record by ID.
- **REST API:** All operations are accessible via HTTP endpoints for integration with UIs or other services.
- **In-memory Database:** Uses H2 for fast setup and easy testing.

## Endpoints

| Method | Endpoint                | Description                     |
|--------|------------------------ |---------------------------------|
| GET    | /api/employees          | List all employees              |
| POST   | /api/employees          | Add a new employee              |
| GET    | /api/employees/{id}     | Get employee by ID              |
| PUT    | /api/employees/{id}     | Update employee details         |
| DELETE | /api/employees/{id}     | Delete employee by ID           |

## Setup & Run

1. **Clone the repository.**
2. **Build and run the app:**
    ```bash
    mvn spring-boot:run
    ```
3. **Access the API:**  
   The application will run at `http://localhost:8080`.

4. **H2 Database Console:**  
   Visit `http://localhost:8080/h2-console`  
   - JDBC URL: `jdbc:h2:mem:employeedb`  
   - User: `sa` (no password)

## Scope

This project demonstrates the core principles of building RESTful APIs with Spring Boot and JPA. The scope is intentionally kept simple for educational and demonstration purposes, and includes:

- Basic CRUD operations for employee management.
- Simple data model: Employee (ID, Name, Department, Salary).
- No authentication or authorization (for simplicity).
- No advanced business logic or workflows.
- No frontend; API-only backend for easy integration.

**Potential Extensions:**
- Add authentication (e.g. JWT, OAuth2).
- Add more fields or entities (Departments, Roles).
- Integrate with a persistent database (MySQL, PostgreSQL).
- Build a frontend using React, Angular, or Vue.
- Add input validation and error handling.

## License

This project is open source and available under the [MIT License](LICENSE).