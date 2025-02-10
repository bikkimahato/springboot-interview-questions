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

## Spring Boot Core
### Table of Contents
| No. | Questions |
| --- | --------- |
| 1   | [What are the main features of Spring Boot and how does it simplify development compared to the traditional Spring framework?](#1-what-are-the-main-features-of-spring-boot-and-how-does-it-simplify-development-compared-to-the-traditional-spring-framework) |
| 2   | [Explain the concept of auto-configuration in Spring Boot. How does it work and how can you customize it?](#2-explain-the-concept-of-auto-configuration-in-spring-boot-how-does-it-work-and-how-can-you-customize-it) |
| 3   | [What are Spring Boot Starters and how do they help in building Spring Boot applications?](#3-what-are-spring-boot-starters-and-how-do-they-help-in-building-spring-boot-applications) |
| 4   | [How does Spring Boot handle externalized configuration? Explain the role of `application.properties` and `application.yml`.](#4-how-does-spring-boot-handle-externalized-configuration-explain-the-role-of-applicationproperties-and-applicationyml) |
| 5   | [What is Spring Boot Actuator? What are some of the key endpoints provided by Actuator?](#5-what-is-spring-boot-actuator-what-are-some-of-the-key-endpoints-provided-by-actuator) |
| 6   | [How can you enable and use Spring Boot DevTools in your application? What are its benefits?](#6-how-can-you-enable-and-use-spring-boot-devtools-in-your-application-what-are-its-benefits) |
| 7   | [Explain the difference between `@RestController` and `@Controller` in Spring Boot.](#7-explain-the-difference-between-restcontroller-and-controller-in-spring-boot) |
| 8   | [How does Spring Boot manage dependencies? Explain the role of the `spring-boot-starter-parent` in dependency management.](#8-how-does-spring-boot-manage-dependencies-explain-the-role-of-the-spring-boot-starter-parent-in-dependency-management) |
| 9   | [What is the purpose of `@SpringBootApplication` annotation? How does it work internally?](#9-what-is-the-purpose-of-springbootapplication-annotation-how-does-it-work-internally) |
| 10  | [How can you configure a Spring Boot application to connect to a database? What are some common properties that need to be set?](#10-how-can-you-configure-a-spring-boot-application-to-connect-to-a-database-what-are-some-common-properties-that-need-to-be-set) |
| 11  | [What are Spring Boot profiles and how do you use them to manage different environments?](#11-what-are-spring-boot-profiles-and-how-do-you-use-them-to-manage-different-environments) |
| 12  | [How do you handle exceptions globally in a Spring Boot application? Explain the use of `@ControllerAdvice`.](#12-how-do-you-handle-exceptions-globally-in-a-spring-boot-application-explain-the-use-of-controlleradvice) |
| 13  | [What is the use of `@ConfigurationProperties` in Spring Boot? How does it help in managing configuration?](#13-what-is-the-use-of-configurationproperties-in-spring-boot-how-does-it-help-in-managing-configuration) |
| 14  | [How can you secure a Spring Boot application using Spring Security? Provide an example.](#14-how-can-you-secure-a-spring-boot-application-using-spring-security-provide-an-example) |
| 15  | [Explain the concept of embedded servers in Spring Boot. How can you configure and use different embedded servers like Tomcat, Jetty, and Undertow?](#15-explain-the-concept-of-embedded-servers-in-spring-boot-how-can-you-configure-and-use-different-embedded-servers-like-tomcat-jetty-and-undertow) |

## Spring Boot Basic Interview Questions and Answers
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

## Spring Boot Core Interview Questions and Answers
### 1. What are the main features of Spring Boot and how does it simplify development compared to the traditional Spring framework?
Spring Boot is designed to simplify the development of Spring-based applications by providing a range of features that streamline configuration and deployment. Some of its main features include:

- **Auto-configuration**: Automatically configures Spring applications based on the dependencies present in the classpath.
- **Embedded Servers**: Comes with embedded servers like Tomcat, Jetty, and Undertow, reducing the need for complex server configurations.
- **Spring Boot Starters**: Provide a set of convenient dependency descriptors to simplify Maven or Gradle configuration.
- **Spring Boot CLI**: Allows you to run and test Spring Boot applications from the command line.
- **Spring Boot Actuator**: Provides production-ready features such as metrics, health checks, and more.
- **Externalized Configuration**: Supports externalized configuration via `application.properties` or `application.yml` files.
- **DevTools**: Enhances the development experience with features like automatic restarts and live reloads.

### Example
Here's a simple Spring Boot application:

```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@SpringBootApplication
public class MySpringBootApplication {
    public static void main(String[] args) {
        SpringApplication.run(MySpringBootApplication.class, args);
    }
}

@RestController
class MyController {
    @GetMapping("/")
    public String hello() {
        return "Hello, Spring Boot!";
    }
}
```
#### **[⬆ Back to Top](#level--spring-boot-core)**
---

### 2. Explain the concept of auto-configuration in Spring Boot. How does it work and how can you customize it?
Auto-configuration is a key feature of Spring Boot that automatically configures your application based on the dependencies you have added. It eliminates the need for explicit configuration in many cases.

### How it works
Spring Boot scans the classpath for libraries and uses predefined configuration classes to set up beans and other components automatically. The `@EnableAutoConfiguration` annotation (implicitly included in `@SpringBootApplication`) triggers this behavior.

### Customizing Auto-Configuration
You can customize auto-configuration using configuration properties or by defining custom beans. If you need to exclude specific auto-configurations, you can use the `@EnableAutoConfiguration` annotation with the `exclude` attribute.

### Example
To exclude a particular auto-configuration class:

```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.boot.autoconfigure.jdbc.DataSourceAutoConfiguration;

@SpringBootApplication(exclude = {DataSourceAutoConfiguration.class})
public class MySpringBootApplication {
    public static void main(String[] args) {
        SpringApplication.run(MySpringBootApplication.class, args);
    }
}
```
#### **[⬆ Back to Top](#level--spring-boot-core)**
---

### 3. What are Spring Boot Starters and how do they help in building Spring Boot applications?
Spring Boot Starters are a set of convenient dependency descriptors you can include in your application. They provide a curated set of dependencies for specific functionalities, making it easier to set up a new Spring Boot application.

### Example
To create a web application, you can add the `spring-boot-starter-web` dependency:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```

This starter includes dependencies for Spring MVC, Jackson for JSON processing, and an embedded Tomcat server.

#### **[⬆ Back to Top](#level--spring-boot-core)**
---

### 4. How does Spring Boot handle externalized configuration? Explain the role of `application.properties` and `application.yml`.
Spring Boot allows you to externalize your configuration so that you can work with the same application code in different environments. This is done using `application.properties` or `application.yml` files.

### Example
`application.properties`:
```properties
server.port=8081
spring.datasource.url=jdbc:mysql://localhost:3306/mydb
spring.datasource.username=root
spring.datasource.password=secret
```

`application.yml`:
```yaml
server:
  port: 8081
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/mydb
    username: root
    password: secret
```
#### **[⬆ Back to Top](#level--spring-boot-core)**
---

## 5. What is Spring Boot Actuator? What are some of the key endpoints provided by Actuator?
Spring Boot Actuator provides production-ready features for Spring Boot applications, such as monitoring and management capabilities. It includes endpoints that allow you to interact with your application and gather various metrics and information.

### Example
To enable Actuator, add the following dependency:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-actuator</artifactId>
</dependency>
```

### Key Endpoints
- `/actuator/health`: Provides information about the application's health status.
- `/actuator/info`: Displays arbitrary application information.
- `/actuator/metrics`: Exposes various metrics about the application.
- `/actuator/env`: Displays properties from the `Environment`.

#### **[⬆ Back to Top](#level--spring-boot-core)**
---