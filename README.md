# SpringBoot Interview Questions

Welcome to the **SpringBoot Interview Questions** repository! 🎉

This repository is designed to be a comprehensive resource for anyone preparing for a SpringBoot interview. Whether you're a beginner looking to get started or an experienced developer brushing up on your skills, you'll find valuable information here.

## 📖 Introduction

SpringBoot is a powerful framework used to build production-ready applications quickly and easily. With its extensive ecosystem and robust features, it's a popular choice for developers. This repository aims to provide a curated list of interview questions and answers to help you prepare for your next SpringBoot interview.

## 🗂 Questions by Topic

We've organized the questions into various topics to make it easier for you to navigate and find what you're looking for. Each topic is covered in detail, with questions ranging from basic to advanced levels.

### Basic Questions
- What is SpringBoot?
- What are the main features of SpringBoot?
- Explain the SpringBoot architecture.

### Core Concepts
- What is dependency injection?
- How does SpringBoot manage dependencies?
- What is a SpringBoot starter?

### Annotations
- Explain the use of `@SpringBootApplication`.
- What is `@RestController` used for?
- How does `@Autowired` work?

### Configuration
- How do you configure a SpringBoot application?
- What is application.properties?
- Explain the use of `@Configuration` and `@Bean`.

### Data Access
- What is Spring Data JPA?
- How do you configure a data source in SpringBoot?
- Explain the use of `@Repository`.

### Security
- How does Spring Security integrate with SpringBoot?
- What is OAuth2 and how is it used with SpringBoot?
- Explain the use of `@PreAuthorize`.

### Testing
- How do you write unit tests for SpringBoot applications?
- What is the role of `@SpringBootTest`?
- Explain the use of MockMvc in SpringBoot tests.

### Advanced Topics
- What is Spring Cloud?
- How do you implement microservices with SpringBoot?
- Explain the use of SpringBoot Actuator.

## 🙌 Contributing

We welcome contributions from the community! If you have additional questions, answers, or improvements, please feel free to submit a pull request.

---

Happy coding and good luck with your interview preparation! 🚀

---

## Spring Boot Basic
### Table of Contents
| No. | Questions |
| --- | --------- |
| 1   | [What is Spring Boot?](#1-what-is-spring-boot) |
| 2   | [What are the main features of Spring Boot?](#2-what-are-the-main-features-of-spring-boot) |
| 3   | [Explain the Spring Boot architecture.](#3-explain-the-spring-boot-architecture) |
| 4   | [What is the purpose of the `@SpringBootApplication` annotation?](#4-what-is-the-purpose-of-the-springbootapplication-annotation) |
| 5   | [How does Spring Boot simplify dependency management?](#5-how-does-spring-boot-simplify-dependency-management) |
| 6   | [What are Spring Boot Starters and how do they help in development?](#6-what-are-spring-boot-starters-and-how-do-they-help-in-development) |
| 7   | [Explain the concept of "convention over configuration" in Spring Boot.](#7-explain-the-concept-of-convention-over-configuration-in-spring-boot) |
| 8   | [How can you create a Spring Boot application using Spring Initializr?](#8-how-can-you-create-a-spring-boot-application-using-spring-initializr) |
| 9   | [What is the difference between the `application.properties` and `application.yml` files?](#9-what-is-the-difference-between-the-applicationproperties-and-applicationyml-files) |
| 10  | [How do you define a custom configuration in Spring Boot?](#10-how-do-you-define-a-custom-configuration-in-spring-boot) |

## Spring Boot Basic Interview Questions and answers
### 1. What is Spring Boot?

Spring Boot is an open-source framework developed by Pivotal Team (part of VMware) which is used to create stand-alone, production-grade Spring-based applications. It simplifies the setup and development of new Spring applications by providing a range of non-functional features commonly used in applications (such as embedded servers, security, and metrics) out of the box.

**Example:**
```java
// Sample Spring Boot Application
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class MySpringBootApplication {
    public static void main(String[] args) {
        SpringApplication.run(MySpringBootApplication.class, args);
    }
}
```
#### **[⬆ Back to Top](#level--spring-boot-basic)**
---

### 2. What are the main features of Spring Boot?

- **Auto-Configuration**: Automatically configures your Spring application based on the dependencies you have added.
- **Standalone**: Standalone applications that can be run from the command line.
- **Embedded Server**: No need for deploying WAR files, embedded servers like Tomcat, Jetty, etc.
- **Production Ready**: Metrics, health checks, and externalized configuration.
- **Spring Boot Starters**: Set of convenient dependency descriptors to quickly set up a Spring-based project.
- **Spring Boot CLI**: Command-line interface for creating and deploying Spring Boot applications.

**Example:**
```java
// Auto-Configuration Example
import org.springframework.boot.autoconfigure.EnableAutoConfiguration;
import org.springframework.context.annotation.ComponentScan;
import org.springframework.context.annotation.Configuration;

@Configuration
@EnableAutoConfiguration
@ComponentScan
public class MyAutoConfigurationApp {
    public static void main(String[] args) {
        SpringApplication.run(MyAutoConfigurationApp.class, args);
    }
}
```
#### **[⬆ Back to Top](#level--spring-boot-basic)**
---

### 3. Explain the Spring Boot architecture.

Spring Boot architecture is built on top of the Spring Framework. It follows the layered architecture pattern which includes:

- **Presentation Layer**: Handles the HTTP requests and responses.
- **Service Layer**: Contains business logic.
- **Repository Layer**: Deals with database operations.
- **Integration Layer**: Integrates with other services or APIs.

Spring Boot uses the following key components:
- **Spring Core**: Provides dependency injection.
- **Spring MVC**: Provides model-view-controller architecture.
- **Spring Data**: Provides easy data access.
- **Spring Security**: Provides authentication and authorization.
- **Spring Boot Auto Configuration**: Automatically configures application based on dependencies.

**Example:**
```java
// Service Layer Example
import org.springframework.stereotype.Service;

@Service
public class MyService {
    public String getGreeting() {
        return "Hello, World!";
    }
}

// Controller Layer Example
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class MyController {
    private final MyService myService;

    public MyController(MyService myService) {
        this.myService = myService;
    }

    @GetMapping("/greeting")
    public String greeting() {
        return myService.getGreeting();
    }
}
```
#### **[⬆ Back to Top](#level--spring-boot-basic)**
---

### 4. What is the purpose of the `@SpringBootApplication` annotation?

The `@SpringBootApplication` annotation is a combination of three annotations:
- `@Configuration`: Indicates that the class has `@Bean` definition methods.
- `@EnableAutoConfiguration`: Enables Spring Boot’s auto-configuration mechanism.
- `@ComponentScan`: Enables component scanning so that the web controller classes and other components you create are automatically discovered and registered as beans in Spring's application context.

**Example:**
```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class MySpringBootApplication {
    public static void main(String[] args) {
        SpringApplication.run(MySpringBootApplication.class, args);
    }
}
```
#### **[⬆ Back to Top](#level--spring-boot-basic)**
---

### 5. How does Spring Boot simplify dependency management?

Spring Boot simplifies dependency management by providing a set of "starter" dependencies. These starters are a set of convenient dependency descriptors that you can include in your application to get a pre-defined set of libraries.

**Example:**
```xml
<!-- Maven POM Example -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```

With this starter, you get all the necessary dependencies for building a web application, including Spring MVC, Jackson for JSON binding, and an embedded Tomcat server.

#### **[⬆ Back to Top](#level--spring-boot-basic)**
---

### 6. What are Spring Boot Starters and how do they help in development?

Spring Boot Starters are dependency descriptors that can be added to your project to include a set of dependencies. They help in rapid development by reducing the need for manually specifying dependencies in your build configuration.

**Example:**
```xml
<!-- Spring Boot Starter for JPA -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>

<!-- Spring Boot Starter for Web -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```
#### **[⬆ Back to Top](#level--spring-boot-basic)**
---

### 7. Explain the concept of "convention over configuration" in Spring Boot.

"Convention over configuration" is a design paradigm used by Spring Boot to reduce the number of decisions a developer has to make. It provides default configurations based on the context and dependencies of the application, which can be overridden if necessary.

**Example:**
When you add `spring-boot-starter-web` to your project, Spring Boot assumes you want to create a web application and automatically configures Tomcat as the default server.

#### **[⬆ Back to Top](#level--spring-boot-basic)**
---

### 8. How can you create a Spring Boot application using Spring Initializr?

Spring Initializr is a web-based tool provided by Spring to bootstrap a new Spring Boot project. You can select the dependencies and download the project as a ZIP file.

**Steps:**
1. Go to [Spring Initializr](https://start.spring.io/).
2. Select project metadata (Group, Artifact, etc.).
3. Choose dependencies you want to include.
4. Click "Generate" to download the project.

#### **[⬆ Back to Top](#level--spring-boot-basic)**
---

### 9. What is the difference between the `application.properties` and `application.yml` files?

Both `application.properties` and `application.yml` are used for configuring Spring Boot applications. The main difference lies in their format:
- **application.properties**: Key-value pairs.
- **application.yml**: YAML format, which is more readable and supports hierarchical data.

**Example:**
```properties
# application.properties
server.port=8080
spring.datasource.url=jdbc:mysql://localhost:3306/mydb
```

```yaml
# application.yml
server:
  port: 8080
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/mydb
```
#### **[⬆ Back to Top](#level--spring-boot-basic)**
---

### 10. How do you define a custom configuration in Spring Boot?

You can define custom configurations in Spring Boot by creating a class annotated with `@Configuration` and defining beans within it.

**Example:**
```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;

@Configuration
public class MyCustomConfiguration {

    @Bean
    public MyService myService() {
        return new MyServiceImpl();
    }
}
```

In this example, `MyService` is a custom bean that is defined in the configuration class.

#### **[⬆ Back to Top](#level--spring-boot-basic)**
---