# Voting Survey Backend

## Overview
This is a **Spring Boot** backend for a Voting Survey application that allows users to participate in surveys, submit votes, and view results via REST APIs.

## Features
- **User Management**: Register, login, and manage user accounts.
- **Survey Management**: Create, update, and delete surveys.
- **Voting System**: Users can submit votes for different survey options.
- **Result Calculation**: View real-time survey results.
- **REST API**: Provides secure and scalable endpoints.
- **Spring Security**: JWT authentication for secured API access.

## Tech Stack
- **Backend**: Java, Spring Boot
- **Database**: MySQL/PostgreSQL
- **Security**: Spring Security, JWT
- **ORM**: Hibernate/JPA
- **API Docs**: Swagger/OpenAPI

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/voting-survey-backend.git
   cd voting-survey-backend
   ```
2. Configure the database in `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/voting_survey
   spring.datasource.username=root
   spring.datasource.password=yourpassword
   ```
3. Build and run the application:
   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

## API Endpoints
| Method | Endpoint           | Description              |
|--------|-------------------|--------------------------|
| POST   | `/auth/register`  | Register a new user     |
| POST   | `/auth/login`     | User login (JWT Token)  |
| GET    | `/surveys`        | Get all surveys         |
| POST   | `/surveys`        | Create a new survey     |
| POST   | `/votes`          | Submit a vote           |
| GET    | `/results/{id}`   | Get survey results      |

## License
This project is open-source and available under the **MIT License**.
