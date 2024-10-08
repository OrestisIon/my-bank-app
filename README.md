# My First Bank App: REST-based Microservices API in Go 🚀

Welcome to the **my-bank-app** project, a comprehensive demonstration of building scalable and secure microservices using Go! 🛠️

This project is a **banking application** that supports essential banking operations like opening new accounts, making deposits, and handling withdrawals. It implements **Role-Based Access Control (RBAC)** to ensure secure access and data integrity, making it suitable for real-world applications. 🏦🔒

## ✨ Key Features:

- 🏗️ **Hexagonal Architecture**: A clean architecture approach that ensures high modularity, making the service easy to test, maintain, and scale.
- 🔐 **OAuth-based Authentication**: Implements a robust **JWT-based Authentication** system, ensuring secure interactions between clients and the server.
- 🔑 **Role-based Authorization**: Uses RBAC to manage access to resources based on user roles, enhancing security.
- 🧪 **Dependency Injection and Mocking**: Promotes clean code practices with dependency injection and the use of mocks for unit testing, ensuring high code quality.
- ✅ **Fully Tested**: Extensive unit tests for routes and services to ensure reliability and robustness.

## 🚀 Why This Project?

This project showcases my ability to design and develop a modern microservices-based application using Go. With a focus on security, modularity, and testing, it reflects my commitment to delivering high-quality code. It’s a great example of my skills in:

- 🌐 Designing RESTful APIs with a focus on **clean architecture**.
- 🛡️ Implementing **authentication and authorization** mechanisms using JWT.
- 🧑‍💻 Building reliable applications with **thorough testing** using mocks.
- 📈 Developing with **scalability and security** in mind.

## 🔧 Get Started:

Feel free to explore the code and learn how to create a robust microservice in Go! If you have any feedback or want to collaborate, don’t hesitate to reach out. Let’s build something great together! 🤝

## 📚 Tools & Technologies:

- **Programming Language**: Go 🐹
- **Authentication**: JWT, OAuth 🔐
- **Architecture**: Hexagonal 🧱
- **Testing**: Mocks and State-based Tests 🧪
- **Database**: SQLx for database operations 💾

Dive into the repository, and let's explore the world of Go-based microservices together! 🌍

##### Run `./start.sh` to download the dependencies and run the the application

To run the application, you have to define the environment variables, default values of the variables are defined inside `start.sh`

- SERVER_ADDRESS    `[IP Address of the machine]`
- SERVER_PORT       `[Port of the machine]`
- DB_USER           `[Database username]`
- DB_PASSWD         `[Database password]`
- DB_ADDR           `[IP address of the database]`
- DB_PORT           `[Port of the database]`
- DB_NAME           `[Name of the database]`

# mysql database
You can use any one of the following procedure to make a database instance, and make the changes to your `start.sh` file accordingly 
1. `docker-compose.yml` file. This contains the init script to generate and tables and insert the default data. You just need to bring the container up

    To start the docker container, run the `docker-compose up` inside the `resources/docker` folder
 
2. `resources/database.sql` this contains the SQL for generating the tables. In case you dont want to use the docker-compose file you can use this file to generate tables and insert the default data

# mocks generator
`./generate-mocks.sh`

# run unit tests
  `./run-tests.sh`
