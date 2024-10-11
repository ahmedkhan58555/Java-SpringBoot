# Spring Boot CRUD Application

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Setup](#setup)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [License](#license)
- [Author](#author)

## Introduction
This **Spring Boot CRUD Application** provides a robust solution for managing employee records. It allows users to perform Create, Read, Update, and Delete (CRUD) operations on employee information through a RESTful API.

## Features
- **User Authentication**: Secure access to the application.
- **CRUD Operations**: Full management of employee records.
- **Pagination**: Efficient handling of large datasets.
- **Sorting**: Easily sort employees by various fields.
- **Exception Handling**: Graceful error responses.
- **Data Validation**: Ensures data integrity during input.

## Technologies Used
| Technology      | Description        |
|-----------------|--------------------|
| **Java**        | Version 17         |
| **Spring Boot** | Version 2.6.7      |
| **Hibernate**   | Version 5.6.5      |
| **MySQL**       | Version 8.0        |
| **Maven**       | Version 3.8.4      |
| **Postman**     | Tool for API testing|

## Installation
To run this application locally, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/ahmedkhan58555/java/spring-crud-application.git
    ```

2. **Navigate to the project directory:**
    ```bash
    cd spring-crud-application
    ```

3. **Open the application in your preferred IDE:**
   - Examples: IntelliJ IDEA, Eclipse, or Spring Tool Suite.

4. **Configure the application properties:**
   - Update the `src/main/resources/application.properties` file to set your database credentials.
   - Example configuration:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
     spring.datasource.username=your_database_username
     spring.datasource.password=your_database_password
     spring.jpa.hibernate.ddl-auto=update
     spring.jpa.show-sql=true
     ```

5. **Install dependencies:**
   - Ensure Maven is installed on your machine.
   - From the project root, run:
     ```bash
     mvn install
     ```

6. **Run the application:**
    ```bash
    mvn spring-boot:run
    ```

## Setup
### MySQL Database Setup
To set up the MySQL database for this application:

1. **Install MySQL** if it is not already installed on your machine. You can download it from the [MySQL official website](https://dev.mysql.com/downloads/).

2. **Create a new database** for the application:
   - Open the MySQL command line or a MySQL GUI client (like MySQL Workbench).
   - Run the following SQL command:
     ```sql
     CREATE DATABASE your_database_name;
     ```

3. **Create the necessary tables**: The application will automatically create the necessary tables based on the entity classes when you run it for the first time, thanks to Hibernate's `ddl-auto` property set to `update`.

## Usage
Once the application is running, you can use Postman or any REST client to interact with the API.

### Example requests:
- **Create Employee**:
    - Method: `POST`
    - URL: `/api/employees`
- **Get All Employees**:
    - Method: `GET`
    - URL: `/api/employees`
- **Get Employee by ID**:
    - Method: `GET`
    - URL: `/api/employees/{id}`
- **Update Employee**:
    - Method: `PUT`
    - URL: `/api/employees/{id}`
- **Delete Employee**:
    - Method: `DELETE`
    - URL: `/api/employees/{id}`

## API Endpoints
| Method | Endpoint               | Description                     |
|--------|------------------------|---------------------------------|
| POST   | /api/employees         | Create a new employee           |
| GET    | /api/employees         | Retrieve all employees          |
| GET    | /api/employees/{id}    | Retrieve employee by ID         |
| PUT    | /api/employees/{id}    | Update an existing employee     |
| DELETE | /api/employees/{id}    | Delete an employee              |

## License
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## Author
**Muhammad Ahmed Khan**  
GitHub: [ahmedkhan58555](https://github.com/ahmedkhan58555)
Feel free to reach out through GitHub for any inquiries or feedback!


## Future Enhancements

Planning to integrate a front-end framework, most likely Angular, into this project soon.
