# Task Management Application

This is a simple Task Management application built with Spring Boot. The application allows users to perform CRUD (Create, Read, Update, Delete) operations on tasks.

## Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)

## Features

- Create new tasks
- Retrieve all tasks
- Retrieve completed tasks
- Retrieve incomplete tasks
- Update existing tasks
- Delete tasks

## Project Structure

The project structure is as follows:
src
├── main
│ ├── java
│ │ └── com
│ │ └── example
│ │ └── demo
│ │ ├── controllers
│ │ │ └── TaskController.java
│ │ ├── entities
│ │ │ └── Task.java
│ │ ├── repositories
│ │ │ └── TaskRepository.java
│ │ └── services
│ │ └── TaskService.java
│ └── resources
│ └── application.properties
└── test
└── java
└── com
└── example
└── demo
└── DemoApplicationTests.java
## Requirements

- Java 17 or higher
- Maven
- PostgreSQL (or another database of your choice)

## Installation

1. **Clone the repository:**

```bash
git clone https://github.com/saranedaran/todo-list-backend-using-springboot.git
cd demo

2. **Configure the database:**

Update the src/main/resources/application.properties file with your database configuration:

spring.datasource.url=jdbc:postgresql://localhost:5432/yourdatabase
spring.datasource.username=yourusername
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

3. **Build and run the application:**
The application will start on "http://localhost:8080"

## Usage
You can use Postman or any other API client to test the endpoints.

API Endpoints
Create a new task

POST /api/v1/tasks
Request Body:
{
  "task": "Buy groceries",
  "completed": false
}

Get all tasks
GET /api/v1/tasks

Get completed tasks
GET /api/v1/tasks/completed

Get incomplete tasks
GET /api/v1/tasks/incomplete

Update a task
PUT /api/v1/tasks/{id}
Request Body:

{
  "task": "Buy groceries and fruits",
  "completed": true
}

Delete a task
DELETE /api/v1/tasks/{id}

Contributing
Contributions are welcome! Please fork this repository and submit a pull request for any features, bug fixes, or enhancements.

License
This project is licensed under the MIT License. See the LICENSE file for details.
### Explanation of the README

1. **Features**: A summary of what the application can do.
2. **Project Structure**: An overview of the directory structure of the project.
3. **Requirements**: Specifies the tools and software required to run the application.
4. **Installation**: Step-by-step instructions to set up the project locally.
5. **Usage**: Instructions on how to use the application, including a detailed list of API endpoints and their usage.
6. **Contributing**: Information on how others can contribute to the project.
7. **License**: Information about the project's license. 

This README file provides a clear and detailed guide for users and contributors, making it easier to understand and work with your Todo application.






