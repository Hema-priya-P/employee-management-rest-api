# Employee Management REST API

A RESTful web application built using Java and Spring Boot to manage employee records. This project demonstrates CRUD (Create, Read, Update, Delete) operations using Spring Data JPA and an H2 database.

## Features

- Add a new employee
- Retrieve all employees
- Retrieve an employee by ID
- Update employee details
- Delete an employee by ID
- Automatically generate employee IDs
- Persist and retrieve records through Spring Data JPA

## Technologies Used

- **Java:** 21
- **Spring Boot**
- **Spring Web:** REST API development
- **Spring Data JPA:** Database operations
- **H2 Database:** Database storage
- **Maven:** Dependency management and build tool
- **Git and GitHub:** Version control and project hosting

## Employee Details

Each employee record contains:

| Field        | Description                |
| ------------ | -------------------------- |
| `id`         | Unique employee identifier |
| `name`       | Employee name              |
| `department` | Employee department        |
| `salary`     | Employee salary            |

## REST API Endpoints

Base URL: `http://localhost:8080/api/employees`

| Method | Endpoint              | Description                |
| ------ | --------------------- | -------------------------- |
| POST   | `/api/employees`      | Add an employee            |
| GET    | `/api/employees`      | Retrieve all employees     |
| GET    | `/api/employees/{id}` | Retrieve an employee by ID |
| PUT    | `/api/employees/{id}` | Update an employee         |
| DELETE | `/api/employees/{id}` | Delete an employee         |

## Example Requests

### 1. Add an Employee

**POST** `/api/employees`

Request body:

```json
{
  "name": "Priya",
  "department": "IT",
  "salary": 35000
}
```

### 2. Retrieve All Employees

**GET** `/api/employees`

### 3. Retrieve an Employee by ID

**GET** `/api/employees/1`

### 4. Update an Employee

**PUT** `/api/employees/1`

Request body:

```json
{
  "name": "Priya",
  "department": "Development",
  "salary": 40000
}
```

### 5. Delete an Employee

**DELETE** `/api/employees/1`

## How to Run the Project

### Prerequisites

- Java Development Kit (JDK) 21
- Git
- An internet connection for downloading Maven dependencies

### Setup Instructions

1. Clone the repository:

   ```bash
   git clone https://github.com/Hema-priya-P/employee-management-rest-api.git
   ```

2. Navigate to the project directory:

   ```bash
   cd employee-management-rest-api
   ```

3. Run the application on Windows using the Maven wrapper:

   ```bat
   mvnw.cmd spring-boot:run
   ```

4. Once the application starts, access the API at:

   `http://localhost:8080/api/employees`

Replace `YOUR-USERNAME` with your GitHub username in the clone command.

## Database

This project uses the H2 database with Spring Data JPA. The current in-memory configuration may clear employee records when the application restarts.

## Learning Outcomes

- Developing RESTful APIs using Spring Boot
- Implementing CRUD operations
- Working with Spring Data JPA repositories
- Mapping HTTP requests to controller methods
- Handling JSON request and response data
- Managing a Java project with Maven and Git

## Future Enhancements

- Configure persistent database storage
- Improve exception handling and HTTP status codes
- Add input validation
- Write automated unit and integration tests
- Add API documentation using Swagger/OpenAPI

## Author
Hema-priya-P
This project was developed as part of my learning journey in Java, Spring Boot, and REST API development.
