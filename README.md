# Spring HelloWorld Application (BridgeLabz)

## Project Overview

This project demonstrates the fundamentals of **Spring Boot application development** using a simple HelloWorld application. The objective is to understand the core components of Spring Boot such as controllers, REST APIs, MVC architecture, and Thymeleaf templating.

The project is implemented as part of the **BridgeLabz Spring Introduction module** and is structured using **Use Cases (UCs)** to gradually build the application.

---

# Technologies Used

* Java 17
* Spring Boot
* Maven
* Thymeleaf
* Spring Web MVC
* VS Code / STS IDE

---

# Project Structure

```
spring-helloworld-app
│
├── pom.xml
│
└── src
    └── main
        ├── java
        │   └── com
        │       └── example
        │           └── helloworld
        │               │
        │               ├── SpringHelloworldApplication.java
        │               │
        │               └── controller
        │                   ├── HelloWebController.java
        │                   └── HelloRestController.java
        │
        └── resources
            │
            ├── application.properties
            │
            └── templates
                └── message.html
```

---

# Use Cases Implemented

## UC1 – Create HelloWorld Spring Boot Application

A basic Spring Boot application is created using Spring Initializr.
The main class starts the Spring Boot application.

**File**

```
SpringHelloworldApplication.java
```

This file contains the `@SpringBootApplication` annotation and the `main()` method used to launch the application.

---

## UC2 – MVC Controller with Thymeleaf

A Spring MVC controller is created that sends data to an HTML page using **Thymeleaf template engine**.

**Controller**

```
HelloWebController.java
```

Endpoint:

```
http://localhost:8080/web/message
```

The controller sends a message to the Thymeleaf template.

**View**

```
message.html
```

This page displays the message using Thymeleaf expression.

---

## UC3 – REST Controller

A REST endpoint is created to return a simple text response.

**Controller**

```
HelloRestController.java
```

Endpoint:

```
http://localhost:8080
```

Output:

```
Hello from BridgeLabz
```

---

## UC4 – Run Application in VS Code

The Spring Boot application can be executed using Maven or directly from the IDE.

---

# How to Run the Project

Navigate to the project directory:

```
cd spring-helloworld-app
```

Run the application using Maven:

```
mvn spring-boot:run
```

Alternatively, build the project and run the JAR file:

```
mvn clean install
java -jar target/spring-helloworld-app-0.0.1-SNAPSHOT.jar
```

---

# Testing the Application

### REST Endpoint

Open in browser:

```
http://localhost:8080
```

Expected Output:

```
Hello from BridgeLabz
```

---

### MVC Web Page

```
http://localhost:8080/web/message
```

Expected Output:

```
Hello from BridgeLabz
```

(displayed through Thymeleaf template)

---

# Git Branch Structure

Each use case is implemented in a separate feature branch.

```
feature/UC1-spring-helloworld
feature/UC2-thymeleaf-view
feature/UC3-rest-controller
feature/UC4-run-app-vscode
```

---

# Learning Outcomes

After completing this project you will understand:

* Spring Boot project setup
* Spring Boot application lifecycle
* REST controllers
* MVC controllers
* Thymeleaf template engine
* Running Spring Boot applications using Maven

---

# Author

Tanmay Bhosale
