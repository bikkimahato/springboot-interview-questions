# SpringBoot Interview Questions

![SpringBoot Logo](https://miro.medium.com/v2/resize:fit:640/format:webp/1*ljHUhFnaBissdRBe7DIo6g.png)

Welcome to the **SpringBoot Interview Questions** repository! 🎉

This repository is designed to be a comprehensive resource for anyone preparing for a SpringBoot interview. Whether you're a beginner looking to get started or an experienced developer brushing up on your skills, you'll find valuable information here.

## 📖 Introduction

SpringBoot is a powerful framework used to build production-ready applications quickly and easily. With its extensive ecosystem and robust features, it's a popular choice for developers. This repository aims to provide a curated list of interview questions and answers to help you prepare for your next SpringBoot interview.

## 🗂 Questions by Topic

We've organized the questions into various topics to make it easier for you to navigate and find what you're looking for. Each topic is covered in detail, with questions ranging from basic to advanced levels.

### [Basic Questions](#spring-boot-basic)
- What is SpringBoot?
- What are the main features of SpringBoot?
- Explain the SpringBoot architecture.

### [Core Concepts](#spring-boot-core)
- What is dependency injection?
- How does SpringBoot manage dependencies?
- What is a SpringBoot starter?

### [Annotations](#spring-boot-annotations)
- Explain the use of `@SpringBootApplication`.
- What is `@RestController` used for?
- How does `@Autowired` work?

### [Configuration](#spring-boot-configuration)
- How do you configure a SpringBoot application?
- What is application.properties?
- Explain the use of `@Configuration` and `@Bean`.

### [Data Access](#spring-boot-data-access)
- What is Spring Data JPA?
- How do you configure a data source in SpringBoot?
- Explain the use of `@Repository`.

### [Security](#spring-boot-security)
- How does Spring Security integrate with SpringBoot?
- What is OAuth2 and how is it used with SpringBoot?
- Explain the use of `@PreAuthorize`.

### [Testing](#spring-boot-security)
- How do you write unit tests for SpringBoot applications?
- What is the role of `@SpringBootTest`?
- Explain the use of MockMvc in SpringBoot tests.

### [Advanced Topics](#spring-boot-advanced)
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

## Spring Boot Annotations
### Table of Contents
| No. | Questions |
| --- | --------- |
| 1   | [What is the purpose of the `@SpringBootApplication` annotation in Spring Boot? Explain its components.](#1-what-is-the-purpose-of-the-springbootapplication-annotation-in-spring-boot-explain-its-components) |
| 2   | [How does the `@RestController` annotation differ from the `@Controller` annotation in Spring Boot?](#2-how-does-the-restcontroller-annotation-differ-from-the-controller-annotation-in-spring-boot) |
| 3   | [Explain the use of `@Autowired` in Spring Boot. How does it work, and what are its alternatives?](#3-explain-the-use-of-autowired-in-spring-boot-how-does-it-work-and-what-are-its-alternatives) |
| 4   | [What is the role of the `@Configuration` annotation in Spring Boot? Can you provide an example?](#4-what-is-the-role-of-the-configuration-annotation-in-spring-boot-can-you-provide-an-example) |
| 5   | [Describe the `@Value` annotation and its usage in Spring Boot applications.](#5-describe-the-value-annotation-and-its-usage-in-spring-boot-applications) |
| 6   | [Can you explain the `@Component`, `@Service`, and `@Repository` annotations? How are they different from each other?](#6-can-you-explain-the-component-service-and-repository-annotations-how-are-they-different-from-each-other) |
| 7   | [What is the `@EnableAutoConfiguration` annotation, and how does it function in a Spring Boot application?](#7-what-is-the-enableautoconfiguration-annotation-and-how-does-it-function-in-a-spring-boot-application) |
| 8   | [Explain the purpose of the `@ComponentScan` annotation and how it is used in Spring Boot.](#8-explain-the-purpose-of-the-componentscan-annotation-and-how-it-is-used-in-spring-boot) |
| 9   | [How does the `@Conditional` annotation work in Spring Boot? Provide an example of its usage.](#9-how-does-the-conditional-annotation-work-in-spring-boot-provide-an-example-of-its-usage) |
| 10  | [What is the `@RequestMapping` annotation used for in Spring Boot? How does it differ from `@GetMapping`, `@PostMapping`, etc.?](#10-what-is-the-requestmapping-annotation-used-for-in-spring-boot-how-does-it-differ-from-getmapping-postmapping-etc) |
| 11  | [Describe the `@Entity` annotation and its role in Spring Boot applications using JPA.](#11-describe-the-entity-annotation-and-its-role-in-spring-boot-applications-using-jpa) |
| 12  | [What is the `@Transactional` annotation, and how is it used in Spring Boot applications?](#12-what-is-the-transactional-annotation-and-how-is-it-used-in-spring-boot-applications) |
| 13  | [Explain the `@Bean` annotation and its usage in a Spring Boot application.](#13-explain-the-bean-annotation-and-its-usage-in-a-spring-boot-application) |
| 14  | [How does the `@Profile` annotation work in Spring Boot? Provide an example of its usage.](#14-how-does-the-profile-annotation-work-in-spring-boot-provide-an-example-of-its-usage) |
| 15  | [What is the `@SpringBootTest` annotation, and how is it used in writing tests for Spring Boot applications?](#15-what-is-the-springboottest-annotation-and-how-is-it-used-in-writing-tests-for-spring-boot-applications) |

## Spring Boot Configurations
### Table of Contents
| No. | Questions |
| --- | --------- |
| 1   | [What is Spring Boot and how does it differ from the traditional Spring Framework?](#1-what-is-spring-boot-and-how-does-it-differ-from-the-traditional-spring-framework) |
| 2   | [How do you define and use properties in Spring Boot? Explain the use of `application.properties` and `application.yml`.](#2-how-do-you-define-and-use-properties-in-spring-boot-explain-the-use-of-applicationproperties-and-applicationyml) |
| 3   | [What is the purpose of the `@Configuration` annotation in Spring Boot?](#3-what-is-the-purpose-of-the-configuration-annotation-in-spring-boot) |
| 4   | [Explain the concept of auto-configuration in Spring Boot. How does Spring Boot automatically configure your application based on the dependencies present in the classpath?](#4-explain-the-concept-of-auto-configuration-in-spring-boot-how-does-spring-boot-automatically-configure-your-application-based-on-the-dependencies-present-in-the-classpath) |
| 5   | [What is `@Value` annotation and how do you use it to inject properties in Spring Boot?](#5-what-is-value-annotation-and-how-do-you-use-it-to-inject-properties-in-spring-boot) |
| 6   | [How can you externalize configuration in Spring Boot and what are the different ways to do it?](#6-how-can-you-externalize-configuration-in-spring-boot-and-what-are-the-different-ways-to-do-it) |
| 7   | [Explain the difference between `@Configuration` and `@Component`. When would you use one over the other?](#7-explain-the-difference-between-configuration-and-component-when-would-you-use-one-over-the-other) |
| 8   | [What is the purpose of the `@EnableAutoConfiguration` annotation?](#8-what-is-the-purpose-of-the-enableautoconfiguration-annotation) |
| 9   | [How do you create and use custom configuration properties in Spring Boot?](#9-how-do-you-create-and-use-custom-configuration-properties-in-spring-boot) |
| 10  | [What are Spring Profiles and how do you use them to manage different configurations for different environments?](#10-what-are-spring-profiles-and-how-do-you-use-them-to-manage-different-configurations-for-different-environments) |
| 11  | [How do you secure sensitive data in your configuration files, such as passwords and API keys?](#11-how-do-you-secure-sensitive-data-in-your-configuration-files-such-as-passwords-and-api-keys) |
| 12  | [Explain how to configure a Spring Boot application to connect to a database.](#12-explain-how-to-configure-a-spring-boot-application-to-connect-to-a-database) |
| 13  | [What is `spring-boot-starter` and how does it simplify dependency management?](#13-what-is-spring-boot-starter-and-how-does-it-simplify-dependency-management) |
| 14  | [How do you create and register a custom `BeanPostProcessor` in Spring Boot?](#14-how-do-you-create-and-register-a-custom-beanpostprocessor-in-spring-boot) |
| 15  | [How does Spring Boot handle logging and how can you configure it?](#15-how-does-spring-boot-handle-logging-and-how-can-you-configure-it) |

## Spring Boot Data Access
| No. | Questions |
| --- | --------- |
| 1   | [What is Spring Data JPA and how does it simplify data access in Spring Boot applications?](#1-what-is-spring-data-jpa-and-how-does-it-simplify-data-access-in-spring-boot-applications) |
| 2   | [Can you explain the difference between CrudRepository, PagingAndSortingRepository, and JpaRepository in Spring Data JPA?](#2-can-you-explain-the-difference-between-crudrepository-pagingandsortingrepository-and-jparepository-in-spring-data-jpa) |
| 3   | [How do you configure a Spring Boot application to connect to a relational database?](#3-how-do-you-configure-a-spring-boot-application-to-connect-to-a-relational-database) |
| 4   | [What is the purpose of the @Entity annotation in Spring Data JPA?](#4-what-is-the-purpose-of-the-entity-annotation-in-spring-data-jpa) |
| 5   | [How do you handle transactions in Spring Boot?](#5-how-do-you-handle-transactions-in-spring-boot) |
| 6   | [What are some common strategies for handling database migrations in Spring Boot?](#6-what-are-some-common-strategies-for-handling-database-migrations-in-spring-boot) |
| 7   | [How would you implement a custom query method in a Spring Data JPA repository?](#7-how-would-you-implement-a-custom-query-method-in-a-spring-data-jpa-repository) |
| 8   | [What is the difference between EntityManager and Hibernate Session in Spring Boot?](#8-what-is-the-difference-between-entitymanager-and-hibernate-session-in-spring-boot) |
| 9   | [Can you explain the purpose and usage of @Modifying and @Query annotations in Spring Data JPA?](#9-can-you-explain-the-purpose-and-usage-of-modifying-and-query-annotations-in-spring-data-jpa) |
| 10  | [How do you implement pagination and sorting in a Spring Boot application?](#10-how-do-you-implement-pagination-and-sorting-in-a-spring-boot-application) |
| 11  | [What is the N+1 selects problem in JPA, and how do you solve it in Spring Boot?](#11-what-is-the-n+1-selects-problem-in-jpa-and-how-do-you-solve-it-in-spring-boot) |
| 12  | [How do you manage database connections in a Spring Boot application?](#12-how-do-you-manage-database-connections-in-a-spring-boot-application) |
| 13  | [What is the difference between eager and lazy fetching in JPA?](#13-what-is-the-difference-between-eager-and-lazy-fetching-in-jpa) |
| 14  | [How do you handle optimistic locking in JPA?](#14-how-do-you-handle-optimistic-locking-in-jpa) |
| 15  | [What are some best practices for designing and maintaining Spring Data JPA repositories?](#15-what-are-some-best-practices-for-designing-and-maintaining-spring-data-jpa-repositories) |

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
#### **[⬆ Back to Top](#spring-boot-basic)**
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
#### **[⬆ Back to Top](#spring-boot-basic)**
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
#### **[⬆ Back to Top](#spring-boot-basic)**
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
#### **[⬆ Back to Top](#spring-boot-basic)**
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

#### **[⬆ Back to Top](#spring-boot-basic)**
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
#### **[⬆ Back to Top](#spring-boot-basic)**
---

### 7. Explain the concept of "convention over configuration" in Spring Boot.

"Convention over configuration" is a design paradigm used by Spring Boot to reduce the number of decisions a developer has to make. It provides default configurations based on the context and dependencies of the application, which can be overridden if necessary.

**Example:**
When you add `spring-boot-starter-web` to your project, Spring Boot assumes you want to create a web application and automatically configures Tomcat as the default server.

#### **[⬆ Back to Top](#spring-boot-basic)**
---

### 8. How can you create a Spring Boot application using Spring Initializr?

Spring Initializr is a web-based tool provided by Spring to bootstrap a new Spring Boot project. You can select the dependencies and download the project as a ZIP file.

**Steps:**
1. Go to [Spring Initializr](https://start.spring.io/).
2. Select project metadata (Group, Artifact, etc.).
3. Choose dependencies you want to include.
4. Click "Generate" to download the project.

#### **[⬆ Back to Top](#spring-boot-basic)**
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
#### **[⬆ Back to Top](#spring-boot-basic)**
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

#### **[⬆ Back to Top](#spring-boot-basic)**
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
#### **[⬆ Back to Top](#spring-boot-core)**
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
#### **[⬆ Back to Top](#spring-boot-core)**
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

#### **[⬆ Back to Top](#spring-boot-core)**
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
#### **[⬆ Back to Top](#spring-boot-core)**
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

#### **[⬆ Back to Top](#spring-boot-core)**
---

### 6. How can you enable and use Spring Boot DevTools in your application? What are its benefits?
Spring Boot DevTools provides a set of tools that improve the development experience. It includes features like automatic restarts, live reload, and configurations for a fast feedback loop.

### Enabling DevTools
Add the following dependency to your `pom.xml`:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-devtools</artifactId>
    <optional>true</optional>
</dependency>
```

### Benefits
- **Automatic Restart**: Automatically restarts the application whenever files on the classpath change.
- **Live Reload**: Automatically refreshes the browser when resources change.
- **Configurations**: Provides development-time configurations, such as disabling caching.

#### **[⬆ Back to Top](#spring-boot-core)**
---

### 7. Explain the difference between `@RestController` and `@Controller` in Spring Boot.
`@RestController` and `@Controller` are annotations used to define controllers in Spring Boot, but they serve different purposes.

- **@Controller**: Used to define a controller class that handles web requests and returns view names. It's typically used in conjunction with view technologies like Thymeleaf or JSP.
- **@RestController**: A convenience annotation that combines `@Controller` and `@ResponseBody`. It indicates that the controller's methods should return JSON or XML data directly to the client.

### Example
`@Controller`:
```java
@Controller
public class MyController {
    @GetMapping("/hello")
    public String hello(Model model) {
        model.addAttribute("message", "Hello, Spring Boot!");
        return "hello";
    }
}
```

`@RestController`:
```java
@RestController
public class MyRestController {
    @GetMapping("/hello")
    public String hello() {
        return "Hello, Spring Boot!";
    }
}
```
#### **[⬆ Back to Top](#spring-boot-core)**
---

## 8. How does Spring Boot manage dependencies? Explain the role of the `spring-boot-starter-parent` in dependency management.
Spring Boot simplifies dependency management by providing a set of "starter" dependencies that you can include in your project. These starters bring in a curated set of dependencies to support specific functionalities.

### `spring-boot-starter-parent`
The `spring-boot-starter-parent` is a special starter that provides default configurations for your project, including dependency versions, plugin configurations, and other settings.

### Example
In your `pom.xml`:
```xml
<parent>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-parent</artifactId>
    <version>2.5.4</version>
</parent>

<dependencies>
    <!-- Spring Boot Starter Web for building web applications -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
    </dependency>
</dependencies>
```
#### **[⬆ Back to Top](#spring-boot-core)**
---

### 9. What is the purpose of `@SpringBootApplication` annotation? How does it work internally?
The `@SpringBootApplication` annotation is a convenience annotation that combines three commonly used annotations:

- `@Configuration`: Indicates that the class can be used by the Spring IoC container as a source of bean definitions.
- `@EnableAutoConfiguration`: Enables Spring Boot's auto-configuration mechanism.
- `@ComponentScan`: Enables component scanning, allowing Spring to find and register beans within the package.

### Example
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
#### **[⬆ Back to Top](#spring-boot-core)**
---

### 10. How can you configure a Spring Boot application to connect to a database? What are some common properties that need to be set?
Spring Boot simplifies database configuration by providing default settings and allowing you to override them using properties in `application.properties` or `application.yml`.

### Example
`application.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/mydb
spring.datasource.username=root
spring.datasource.password=secret
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.hibernate.ddl-auto=update
```

`application.yml`:
```yaml
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/mydb
    username: root
    password: secret
    driver-class-name: com.mysql.cj.jdbc.Driver
  jpa:
    hibernate:
      ddl-auto: update
```
#### **[⬆ Back to Top](#spring-boot-core)**
---

### 11. What are Spring Boot profiles and how do you use them to manage different environments?
Spring Boot profiles provide a way to segregate parts of your application configuration and make it only available in certain environments. This allows you to define environment-specific properties and beans.

### Example
Define profile-specific properties in `application-{profile}.properties` or `application-{profile}.yml`.

`application-dev.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/devdb
spring.datasource.username=devuser
spring.datasource.password=devpass
```

`application-prod.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/proddb
spring.datasource.username=produser
spring.datasource.password=prodpass
```

Activate a profile using the `spring.profiles.active` property:
```properties
spring.profiles.active=dev
```

Or set it as a JVM argument:
```sh
java -jar myapp.jar --spring.profiles.active=prod
```
#### **[⬆ Back to Top](#spring-boot-core)**
---

### 12. How do you handle exceptions globally in a Spring Boot application? Explain the use of `@ControllerAdvice`.
Spring Boot allows you to handle exceptions globally using the `@ControllerAdvice` annotation. This annotation is used to define a class that handles exceptions across all controllers.

### Example
```java
import org.springframework.http.HttpStatus;
import org.springframework.web.bind.annotation.ControllerAdvice;
import org.springframework.web.bind.annotation.ExceptionHandler;
import org.springframework.web.bind.annotation.ResponseStatus;
import org.springframework.web.servlet.mvc.method.annotation.ResponseEntityExceptionHandler;

@ControllerAdvice
public class GlobalExceptionHandler extends ResponseEntityExceptionHandler {
    
    @ExceptionHandler(ResourceNotFoundException.class)
    @ResponseStatus(HttpStatus.NOT_FOUND)
    public String handleResourceNotFoundException(ResourceNotFoundException ex) {
        return ex.getMessage();
    }
    
    @ExceptionHandler(Exception.class)
    @ResponseStatus(HttpStatus.INTERNAL_SERVER_ERROR)
    public String handleGenericException(Exception ex) {
        return "An unexpected error occurred: " + ex.getMessage();
    }
}
```
#### **[⬆ Back to Top](#spring-boot-core)**
---

### 13. What is the use of `@ConfigurationProperties` in Spring Boot? How does it help in managing configuration?
The `@ConfigurationProperties` annotation is used to bind external configuration properties to a Java class. It allows you to map properties from `application.properties` or `application.yml` files to a POJO.

### Example
Define a configuration properties class:
```java
import org.springframework.boot.context.properties.ConfigurationProperties;
import org.springframework.stereotype.Component;

@Component
@ConfigurationProperties(prefix = "app")
public class AppProperties {
    private String name;
    private String version;

    // getters and setters
}
```

`application.properties`:
```properties
app.name=MyApp
app.version=1.0.0
```

Access the properties in a Spring component:
```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class AppController {

    @Autowired
    private AppProperties appProperties;

    @GetMapping("/info")
    public String getAppInfo() {
        return "Name: " + appProperties.getName() + ", Version: " + appProperties.getVersion();
    }
}
```
#### **[⬆ Back to Top](#spring-boot-core)**
---

### 14. How can you secure a Spring Boot application using Spring Security? Provide an example.
Spring Security provides comprehensive security services for Java applications. It is highly customizable and can be used to secure a Spring Boot application.

### Example
Add the Spring Security dependency:
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>
```

Create a security configuration class:
```java
import org.springframework.context.annotation.Bean;
import org.springframework.security.config.annotation.web.builders.HttpSecurity;
import org.springframework.security.config.annotation.web.configuration.EnableWebSecurity;
import org.springframework.security.config.annotation.web.configuration.WebSecurityConfigurerAdapter;
import org.springframework.security.crypto.bcrypt.BCryptPasswordEncoder;
import org.springframework.security.crypto.password.PasswordEncoder;

@EnableWebSecurity
public class SecurityConfig extends WebSecurityConfigurerAdapter {

    @Override
    protected void configure(HttpSecurity http) throws Exception {
        http
            .authorizeRequests()
                .antMatchers("/public/**").permitAll()
                .anyRequest().authenticated()
                .and()
            .formLogin().permitAll()
                .and()
            .logout().permitAll();
    }

    @Bean
    public PasswordEncoder passwordEncoder() {
        return new BCryptPasswordEncoder();
    }
}
```
#### **[⬆ Back to Top](#spring-boot-core)**
---

### 15. Explain the concept of embedded servers in Spring Boot. How can you configure and use different embedded servers like Tomcat, Jetty, and Undertow?
Spring Boot includes embedded servers, allowing you to run web applications without needing an external server. By default, Spring Boot uses Tomcat as the embedded server, but you can also use Jetty or Undertow.

### Example
To use Jetty instead of Tomcat, exclude the Tomcat dependency and include the Jetty dependency:
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
    <exclusions>
        <exclusion>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-tomcat</artifactId>
        </exclusion>
    </exclusions>
</dependency>

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-jetty</artifactId>
</dependency>
```
#### **[⬆ Back to Top](#spring-boot-core)**
---

## Spring Boot Annotations Interview Questions and Answers
### 1. What is the purpose of the `@SpringBootApplication` annotation in Spring Boot? Explain its components.

The `@SpringBootApplication` annotation is a convenient annotation that combines three crucial annotations: `@Configuration`, `@EnableAutoConfiguration`, and `@ComponentScan`. It is used to mark the main class of a Spring Boot application.

Components:
- `@Configuration`: Indicates that the class can be used by the Spring IoC container as a source of bean definitions.
- `@EnableAutoConfiguration`: Tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings.
- `@ComponentScan`: Enables component-scanning so that web controllers and other components you create will be automatically discovered and registered as beans in the Spring application context.

Example:
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
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 2. How does the `@RestController` annotation differ from the `@Controller` annotation in Spring Boot?

The `@RestController` annotation is a specialized version of the `@Controller` annotation. It includes the `@Controller` and `@ResponseBody` annotations, meaning that it is a convenience annotation for creating RESTful web services.

- `@Controller`: Used to define a controller class where `@RequestMapping` methods are used to map web requests to specific handler methods. It returns a view name which is resolved to an actual view.
- `@RestController`: Used to create RESTful web services. It combines `@Controller` and `@ResponseBody`, meaning that it returns the response directly as JSON or XML instead of rendering a view.

Example:
```java
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class MyRestController {
    @GetMapping("/hello")
    public String hello() {
        return "Hello, World!";
    }
}
```
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 3. Explain the use of `@Autowired` in Spring Boot. How does it work, and what are its alternatives?

`@Autowired` is used for automatic dependency injection. It allows Spring to resolve and inject collaborating beans into your bean. When `@Autowired` is used on a constructor, setter, or field, the Spring framework injects the required dependency.

How it works:
- Field Injection: Spring injects the dependency directly into the field.
- Setter Injection: Spring injects the dependency via a setter method.
- Constructor Injection: Spring injects the dependency via a constructor.

Alternatives:
- `@Inject` (from javax.inject): Similar to `@Autowired`, but it is part of the JSR-330 specification.
- `@Resource` (from javax.annotation): Can be used for dependency injection and provides more control over the injection process.

Example (Field Injection):
```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Component;

@Component
public class MyService {
    @Autowired
    private MyRepository myRepository;

    public void doSomething() {
        myRepository.save(new MyEntity());
    }
}
```
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 4. What is the role of the `@Configuration` annotation in Spring Boot? Can you provide an example?

The `@Configuration` annotation indicates that the class has `@Bean` definition methods. Spring container uses this class to register beans and configure them using Spring's IoC container.

Role:
- It is used to define beans using `@Bean` annotated methods.
- It helps in separating the configuration from the main application logic.

Example:
```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;

@Configuration
public class AppConfig {
    @Bean
    public MyService myService() {
        return new MyService();
    }
}
```
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 5. Describe the `@Value` annotation and its usage in Spring Boot applications.

The `@Value` annotation is used to inject values into fields in Spring-managed beans. It can be used to inject values from property files, system properties, environment variables, and more.

Usage:
- Injecting values from application properties.
- Injecting default values if the property is not found.
- Injecting system properties or environment variables.

Example:
```java
import org.springframework.beans.factory.annotation.Value;
import org.springframework.stereotype.Component;

@Component
public class MyComponent {
    @Value("${my.property:default_value}")
    private String myProperty;

    public void displayProperty() {
        System.out.println("Property value: " + myProperty);
    }
}
```
In this example, `${my.property:default_value}` means that the value of `my.property` is injected, and if it is not found, `default_value` is used.

#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 6. Can you explain the `@Component`, `@Service`, and `@Repository` annotations? How are they different from each other?

The `@Component`, `@Service`, and `@Repository` annotations are all used to define beans in Spring, but they serve different purposes.

- `@Component`: A generic stereotype for any Spring-managed component. It is the parent annotation for `@Service` and `@Repository`.
- `@Service`: A specialization of `@Component` used to define service layer beans. It is used to annotate classes that perform service tasks, typically containing business logic.
- `@Repository`: A specialization of `@Component` used to define data access layer beans. It is used to annotate classes that interact with the database and often involve CRUD operations.

Example:
```java
import org.springframework.stereotype.Component;
import org.springframework.stereotype.Service;
import org.springframework.stereotype.Repository;

@Component
public class MyComponent {
    public void performTask() {
        System.out.println("Component task");
    }
}

@Service
public class MyService {
    public void performService() {
        System.out.println("Service task");
    }
}

@Repository
public class MyRepository {
    public void save(Object entity) {
        System.out.println("Saving entity");
    }
}
```
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 7. What is the `@EnableAutoConfiguration` annotation, and how does it function in a Spring Boot application?

The `@EnableAutoConfiguration` annotation tells Spring Boot to automatically configure your application based on the dependencies you have added. It enables auto-configuration, which attempts to guess and configure beans you are likely to need.

Function:
- It scans the classpath and configures beans for many common application tasks.
- It reduces the need for explicit configuration by the developer.

Example:
```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.EnableAutoConfiguration;
import org.springframework.context.annotation.ComponentScan;

@EnableAutoConfiguration
@ComponentScan
public class MySpringBootApplication {
    public static void main(String[] args) {
        SpringApplication.run(MySpringBootApplication.class, args);
    }
}
```
In practice, `@SpringBootApplication` (which includes `@EnableAutoConfiguration`) is preferred over using `@EnableAutoConfiguration` directly.

#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 8. Explain the purpose of the `@ComponentScan` annotation and how it is used in Spring Boot.

The `@ComponentScan` annotation is used to specify the base packages to scan for Spring components. It tells Spring where to look for components, configurations, and services.

Purpose:
- It helps in discovering and registering beans with the Spring context.
- It is typically used in conjunction with `@Configuration` or `@SpringBootApplication`.

Example:
```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.context.annotation.ComponentScan;

@SpringBootApplication
@ComponentScan(basePackages = "com.example.myapp")
public class MySpringBootApplication {
    public static void main(String[] args) {
        SpringApplication.run(MySpringBootApplication.class, args);
    }
}
```
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 9. How does the `@Conditional` annotation work in Spring Boot? Provide an example of its usage.

The `@Conditional` annotation is used to conditionally include a bean or configuration only if a certain condition is met. It is often used with custom conditions.

Usage:
- It allows beans to be registered conditionally based on the presence or absence of certain classes, properties, or other conditions.

Example:
```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Conditional;
import org.springframework.context.annotation.Configuration;

@Configuration
public class MyConfig {
    @Bean
    @Conditional(MyCondition.class)
    public MyService myService() {
        return new MyService();
    }
}

public class MyCondition implements Condition {
    @Override
    public boolean matches(ConditionContext context, AnnotatedTypeMetadata metadata) {
        return context.getEnvironment().containsProperty("my.property");
    }
}
```
In this example, `MyService` will only be registered if the property `my.property` is present in the environment.

#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 10. What is the `@RequestMapping` annotation used for in Spring Boot? How does it differ from `@GetMapping`, `@PostMapping`, etc.?

The `@RequestMapping` annotation is used to map HTTP requests to handler methods of MVC and REST controllers. It can be used at both the class and method levels.

Differences:
- `@RequestMapping`: General-purpose annotation that maps any HTTP request method (GET, POST, PUT, DELETE, etc.).
- `@GetMapping`, `@PostMapping`, etc.: Specialized annotations that are shortcuts for `@RequestMapping(method = RequestMethod.GET)`, `@RequestMapping(method = RequestMethod.POST)`, etc.

Example:
```java
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RequestMethod;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class MyController {
    @RequestMapping(value = "/hello", method = RequestMethod.GET)
    public String hello() {
        return "Hello, World!";
    }

    @GetMapping("/greet")
    public String greet() {
        return "Greetings!";
    }
}
```
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 11. Describe the `@Entity` annotation and its role in Spring Boot applications using JPA.

The `@Entity` annotation is used to mark a class as a JPA entity. It indicates that the class is a persistent Java class and is mapped to a database table.

Role:
- It defines the entity and maps it to a database table.
- It is used with other JPA annotations like `@Id`, `@Column`, `@Table`, etc., to define the entity's characteristics.

Example:
```java
import javax.persistence.Entity;
import javax.persistence.Id;

@Entity
public class MyEntity {
    @Id
    private Long id;
    private String name;

    // Getters and Setters
}
```
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 12. What is the `@Transactional` annotation, and how is it used in Spring Boot applications?

The `@Transactional` annotation is used to manage transaction boundaries in Spring applications. It indicates that the method or class should be executed within a transactional context.

Usage:
- It can be applied at the method or class level.
- It ensures that the methods execute within a transaction, and if an exception occurs, the transaction is rolled back.

Example:
```java
import org.springframework.stereotype.Service;
import org.springframework.transaction.annotation.Transactional;

@Service
public class MyService {
    @Transactional
    public void performTransaction() {
        // Business logic that needs to be executed within a transaction
    }
}
```
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 13. Explain the `@Bean` annotation and its usage in a Spring Boot application.

The `@Bean` annotation indicates that a method produces a bean to be managed by the Spring container. It is used within `@Configuration` classes to define beans.

Usage:
- It is used to declare a bean and its configuration details.
- It provides flexibility in defining beans that are not automatically detected by component scanning.

Example:
```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;

@Configuration
public class AppConfig {
    @Bean
    public MyService myService() {
        return new MyService();
    }
}
```
#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 14. How does the `@Profile` annotation work in Spring Boot? Provide an example of its usage.

The `@Profile` annotation is used to indicate that a component or configuration is only active for specific profiles. It helps in managing different configurations for different environments (e.g., development, production).

Usage:
- It can be applied to `@Component` classes, `@Configuration` classes, or individual `@Bean` methods.
- The active profile can be set using the `spring.profiles.active` property.

Example:
```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.context.annotation.Profile;

@Configuration
public class AppConfig {
    @Bean
    @Profile("dev")
    public MyService devMyService() {
        return new MyService("Development Configuration");
    }

    @Bean
    @Profile("prod")
    public MyService prodMyService() {
        return new MyService("Production Configuration");
    }
}
```
In this example, `devMyService` bean will be active in the 'dev' profile, and `prodMyService` bean will be active in the 'prod' profile.

#### **[⬆ Back to Top](#spring-boot-annotations)**
---

### 15. What is the `@SpringBootTest` annotation, and how is it used in writing tests for Spring Boot applications?

The `@SpringBootTest` annotation is used to create an application context for integration tests. It provides a comprehensive environment for testing Spring Boot applications, including auto-configuration, component scanning, and dependencies.

Usage:
- It is used to load the complete application context during tests.
- It can be customized with parameters like `webEnvironment`, `classes`, `properties`, etc.

Example:
```java
import org.junit.jupiter.api.Test;
import org.springframework.boot.test.context.SpringBootTest;

@SpringBootTest
public class MySpringBootTest {
    @Test
    public void contextLoads() {
        // Test to verify the context loads successfully
    }
}
```
In this example, `@SpringBootTest` loads the full application context and verifies that it starts up correctly.

#### **[⬆ Back to Top](#spring-boot-annotations)**
---

## Spring Boot Core Interview Questions and Answers
### 1. What is Spring Boot and how does it differ from the traditional Spring Framework?

**Answer:**
Spring Boot is an extension of the Spring Framework that aims to simplify the development of production-ready applications. It provides a set of conventions and default configurations to reduce boilerplate code and speed up the development process.

### Differences:
- **Auto-Configuration:** Spring Boot automatically configures your application based on the dependencies present in the classpath. In contrast, the traditional Spring Framework requires explicit configuration.
- **Starter POMs:** Spring Boot provides starter dependencies to simplify dependency management. Traditional Spring requires manual dependency management.
- **Embedded Servers:** Spring Boot can embed web servers like Tomcat, Jetty, or Undertow, allowing you to run applications as standalone Java applications. Traditional Spring applications usually require an external web server.
- **Production-Ready Features:** Spring Boot includes features like metrics, health checks, and externalized configuration to support production environments.

### Example:
```java
// Traditional Spring Configuration
@Configuration
public class AppConfig {
    @Bean
    public MyService myService() {
        return new MyServiceImpl();
    }
}

// Spring Boot Configuration
// No explicit configuration needed if MyServiceImpl is a component
@Service
public class MyServiceImpl implements MyService { }
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 2. How do you define and use properties in Spring Boot? Explain the use of `application.properties` and `application.yml`.

**Answer:**
In Spring Boot, you can define properties in two main files: `application.properties` and `application.yml`. These files are used to externalize configuration and can be placed in the `src/main/resources` directory.

### `application.properties` Example:
```properties
server.port=8081
spring.datasource.url=jdbc:mysql://localhost:3306/mydb
spring.datasource.username=root
spring.datasource.password=secret
```

### `application.yml` Example:
```yaml
server:
  port: 8081

spring:
  datasource:
    url: jdbc:mysql://localhost:3306/mydb
    username: root
    password: secret
```

### Using Properties in Code:
You can use the `@Value` annotation to inject properties into your Spring-managed beans.

```java
import org.springframework.beans.factory.annotation.Value;
import org.springframework.stereotype.Component;

@Component
public class MyComponent {

    @Value("${server.port}")
    private int serverPort;

    @Value("${spring.datasource.username}")
    private String dbUsername;

    // getters and setters
}
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 3. What is the purpose of the `@Configuration` annotation in Spring Boot?

**Answer:**
The `@Configuration` annotation in Spring Boot indicates that the class has `@Bean` definition methods. Spring Boot will process this class to generate Spring Beans to be managed by the Spring container.

### Example:
```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;

@Configuration
public class AppConfig {

    @Bean
    public MyService myService() {
        return new MyServiceImpl();
    }
}
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 4. Explain the concept of auto-configuration in Spring Boot. How does Spring Boot automatically configure your application based on the dependencies present in the classpath?

**Answer:**
Spring Boot's auto-configuration mechanism automatically configures your application based on the dependencies present in the classpath. It uses `@EnableAutoConfiguration` and a set of conditional annotations (`@ConditionalOnClass`, `@ConditionalOnMissingBean`, etc.) to apply sensible defaults and configurations for the application.

### Example:
When you add `spring-boot-starter-web` to your project, Spring Boot auto-configures a Tomcat server and the necessary Spring MVC components.

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 5. What is `@Value` annotation and how do you use it to inject properties in Spring Boot?

**Answer:**
The `@Value` annotation is used to inject values into fields of Spring-managed beans. These values can come from property files, system properties, or environment variables.

### Example:
```java
import org.springframework.beans.factory.annotation.Value;
import org.springframework.stereotype.Component;

@Component
public class MyComponent {

    @Value("${server.port}")
    private int serverPort;

    @Value("${spring.datasource.username}")
    private String dbUsername;

    // getters and setters
}
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 6. How can you externalize configuration in Spring Boot and what are the different ways to do it?

**Answer:**
Externalizing configuration means separating configuration from the code. Spring Boot provides several ways to externalize configuration:

1. **Properties and YAML Files:** `application.properties` or `application.yml`.
2. **Environment Variables:** Using environment variables to override configuration properties.
3. **Command-Line Arguments:** Passing properties as arguments when running the application.
4. **Configuration Server:** Using Spring Cloud Config Server to manage configuration centrally.

### Example:
```properties
# application.properties
app.name=MyApp
```

### Command-Line Argument:
```bash
java -jar myapp.jar --app.name=MyApp
```

### Environment Variable:
```bash
export APP_NAME=MyApp
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 7. Explain the difference between `@Configuration` and `@Component`. When would you use one over the other?

**Answer:**
- **`@Configuration`:** Indicates that the class contains one or more `@Bean` methods. It is used for defining beans and their dependencies.
- **`@Component`:** Indicates that an annotated class is a Spring-managed component. It is a generic stereotype for any Spring-managed component.

### Example:
```java
// @Configuration example
@Configuration
public class AppConfig {

    @Bean
    public MyService myService() {
        return new MyServiceImpl();
    }
}

// @Component example
@Component
public class MyServiceImpl implements MyService { }
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 8. What is the purpose of the `@EnableAutoConfiguration` annotation?

**Answer:**
The `@EnableAutoConfiguration` annotation tells Spring Boot to automatically configure your application based on the dependencies present in the classpath. It is typically used in the main application class.

### Example:
```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class MyApplication {
    public static void main(String[] args) {
        SpringApplication.run(MyApplication.class, args);
    }
}
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 9. How do you create and use custom configuration properties in Spring Boot?

**Answer:**
You can create custom configuration properties by defining a properties class and annotating it with `@ConfigurationProperties`. You also need to enable this configuration properties class in your main application class.

### Example:
```properties
# application.properties
myapp.custom.property=CustomValue
```

```java
import org.springframework.boot.context.properties.ConfigurationProperties;
import org.springframework.stereotype.Component;

@Component
@ConfigurationProperties(prefix = "myapp.custom")
public class CustomProperties {

    private String property;

    // getters and setters
}
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 10. What are Spring Profiles and how do you use them to manage different configurations for different environments?

**Answer:**
Spring Profiles allow you to define different configurations for different environments (e.g., development, testing, production). You can use profiles to load specific beans or properties based on the active profile.

### Example:
```properties
# application-dev.properties
server.port=8081

# application-prod.properties
server.port=8082
```

### Activating a Profile:
You can activate a profile using the `spring.profiles.active` property.

```bash
java -jar myapp.jar --spring.profiles.active=dev
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 11. How do you secure sensitive data in your configuration files, such as passwords and API keys?

**Answer:**
To secure sensitive data, you can use the following approaches:

1. **Environment Variables:** Store sensitive data in environment variables and reference them in your configuration.
2. **Encrypted Configuration:** Use tools like Jasypt to encrypt properties in your configuration files.
3. **Configuration Server:** Store sensitive data in a secure configuration server like Spring Cloud Config Server.

### Example using Jasypt:
```properties
# application.properties
spring.datasource.password=ENC(encryptedPassword)
```

```java
import org.jasypt.util.text.BasicTextEncryptor;

public class Encryptor {
    public static void main(String[] args) {
        BasicTextEncryptor textEncryptor = new BasicTextEncryptor();
        textEncryptor.setPassword("secret-key");
        String encryptedPassword = textEncryptor.encrypt("plainPassword");
        System.out.println("Encrypted Password: " + encryptedPassword);
    }
}
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 12. Explain how to configure a Spring Boot application to connect to a database.

**Answer:**
To configure a Spring Boot application to connect to a database, you need to add the necessary dependencies and provide the database connection properties.

### Example:
```xml
<!-- Add MySQL dependency in pom.xml -->
<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <scope>runtime</scope>
</dependency>
```

```properties
# application.properties
spring.datasource.url=jdbc:mysql://localhost:3306/mydb
spring.datasource.username=root
spring.datasource.password=secret
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 13. What is `spring-boot-starter` and how does it simplify dependency management?

**Answer:**
`spring-boot-starter` is a set of convenient dependency descriptors provided by Spring Boot. Each starter includes a curated set of dependencies that you can use to get started quickly. Starters simplify dependency management by aggregating common dependencies into a single, easy-to-use dependency.

### Example:
```xml
<!-- Add the web starter in pom.xml -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 14. How do you create and register a custom `BeanPostProcessor` in Spring Boot?

**Answer:**
A `BeanPostProcessor` allows you to intercept bean creation and perform custom logic before and after the initialization of a bean. You need to implement the `BeanPostProcessor` interface and register it as a Spring bean.

### Example:
```java
import org.springframework.beans.BeansException;
import org.springframework.beans.factory.config.BeanPostProcessor;
import org.springframework.stereotype.Component;

@Component
public class CustomBeanPostProcessor implements BeanPostProcessor {

    @Override
    public Object postProcessBeforeInitialization(Object bean, String beanName) throws BeansException {
        // Custom logic before bean initialization
        return bean;
    }

    @Override
    public Object postProcessAfterInitialization(Object bean, String beanName) throws BeansException {
        // Custom logic after bean initialization
        return bean;
    }
}
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

### 15. How does Spring Boot handle logging and how can you configure it?

**Answer:**
Spring Boot uses `Spring Boot Logging` for logging, which is a combination of SLF4J and Logback. It provides default configurations and allows you to customize logging settings using properties or XML configuration.

### Example:
```properties
# application.properties
logging.level.root=INFO
logging.level.com.myapp=DEBUG
logging.file.name=app.log
logging.pattern.console=%d{yyyy-MM-dd HH:mm:ss} - %msg%n
logging.pattern.file=%d{yyyy-MM-dd HH:mm:ss} - %msg%n
```

### Custom Logback Configuration:
You can create a `logback-spring.xml` file in the `src/main/resources` directory for advanced logging configurations.

```xml
<configuration>
    <appender name="FILE" class="ch.qos.logback.core.FileAppender">
        <file>app.log</file>
        <encoder>
            <pattern>%d{yyyy-MM-dd HH:mm:ss} - %msg%n</pattern>
        </encoder>
    </appender>

    <logger name="com.myapp" level="DEBUG" additivity="false">
        <appender-ref ref="FILE" />
    </logger>

    <root level="INFO">
        <appender-ref ref="FILE" />
    </root>
</configuration>
```
#### **[⬆ Back to Top](#spring-boot-configurations)**
---

## Spring Boot Data Access Interview Questions and Answers
### 1. What is Spring Data JPA and how does it simplify data access in Spring Boot applications?
Spring Data JPA is a part of the larger Spring Data family, which aims to make it easier to work with data access technologies. It provides a repository abstraction over JPA (Java Persistence API) and makes it easier to implement data access layers.

### Advantages:
1. **Boilerplate Reduction**: It reduces the amount of boilerplate code needed for database operations.
2. **Repository Pattern**: Provides a repository pattern with CRUD operations out-of-the-box.
3. **Query Methods**: Supports the creation of query methods directly from the method names.
4. **Pagination and Sorting**: Built-in support for pagination and sorting.
5. **Auditing**: Supports auditing and versioning of entities.

### Example:
```java
// Entity class
@Entity
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    private String name;
    private String email;

    // getters and setters
}

// Repository Interface
public interface UserRepository extends JpaRepository<User, Long> {
    List<User> findByName(String name);
}
```

In this example, `UserRepository` extends `JpaRepository`, which provides basic CRUD operations. The `findByName` method is automatically implemented by Spring Data JPA.

#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 2. Can you explain the difference between CrudRepository, PagingAndSortingRepository, and JpaRepository in Spring Data JPA?
### CrudRepository:
- **Purpose**: Basic CRUD operations (Create, Read, Update, Delete).
- **Methods**: save, findAll, findById, deleteById, etc.

### PagingAndSortingRepository:
- **Purpose**: Extends `CrudRepository` to add methods for pagination and sorting.
- **Methods**: findAll(Pageable pageable), findAll(Sort sort).

### JpaRepository:
- **Purpose**: Extends `PagingAndSortingRepository` to add JPA-specific methods.
- **Methods**: flush, saveAndFlush, deleteInBatch, etc.

### Example:
```java
public interface UserRepository extends JpaRepository<User, Long> {
    List<User> findByName(String name);
}
```

`UserRepository` will have methods from `CrudRepository`, `PagingAndSortingRepository`, and `JpaRepository`.

#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 3. How do you configure a Spring Boot application to connect to a relational database?
### Configuration:
1. **Add Dependency**:
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>
<dependency>
    <groupId>com.h2database</groupId>
    <artifactId>h2</artifactId> <!-- or your database choice -->
</dependency>
```

2. **application.properties**:
```properties
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.username=sa
spring.datasource.password=password
spring.datasource.driver-class-name=org.h2.Driver
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
```
For other databases, replace the URL, username, password, driver, and dialect accordingly.

### Example:
```java
@SpringBootApplication
public class Application {
    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }
}
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 4. What is the purpose of the @Entity annotation in Spring Data JPA?
The `@Entity` annotation specifies that the class is an entity and is mapped to a database table.

### Example:
```java
@Entity
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    private String name;
    private String email;

    // getters and setters
}
```

In this example, the `User` class is mapped to a database table named `User`.

#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 5. How do you handle transactions in Spring Boot?
Transactions in Spring Boot are handled using the `@Transactional` annotation.

### Example:
```java
@Service
public class UserService {

    @Autowired
    private UserRepository userRepository;

    @Transactional
    public void saveUser(User user) {
        userRepository.save(user);
        // Additional transactional logic
    }
}
```

The `@Transactional` annotation ensures that the method is executed within a transaction context.

#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 6. What are some common strategies for handling database migrations in Spring Boot?
### Common Strategies:
1. **Flyway**: Version-based migration tool.
2. **Liquibase**: XML/JSON/YAML-based migration tool.

### Example with Flyway:
1. **Add Dependency**:
```xml
<dependency>
    <groupId>org.flywaydb</groupId>
    <artifactId>flyway-core</artifactId>
</dependency>
```

2. **application.properties**:
```properties
spring.flyway.locations=classpath:db/migration
```

3. **Migration Script**:
```sql
-- V1__Create_user_table.sql
CREATE TABLE user (
    id BIGINT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100)
);
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 7. How would you implement a custom query method in a Spring Data JPA repository?
### Using @Query Annotation:
```java
public interface UserRepository extends JpaRepository<User, Long> {

    @Query("SELECT u FROM User u WHERE u.email = ?1")
    User findByEmail(String email);
}
```

### Using Query Methods:
```java
List<User> findByName(String name);
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 8. What is the difference between EntityManager and Hibernate Session in Spring Boot?
### EntityManager:
- **Standard**: Part of JPA specification.
- **Usage**: Entity lifecycle management in a standard way.

### Hibernate Session:
- **Specific**: Hibernate-specific implementation.
- **Usage**: Additional features not covered by JPA.

### Example:
```java
@Autowired
private EntityManager entityManager;

public User getUser(Long id) {
    return entityManager.find(User.class, id);
}
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 9. Can you explain the purpose and usage of @Modifying and @Query annotations in Spring Data JPA?
### @Query:
Used to define custom queries.

### Example:
```java
@Query("UPDATE User u SET u.name = :name WHERE u.id = :id")
void updateUsername(@Param("id") Long id, @Param("name") String name);
```

### @Modifying:
Used with @Query for update and delete operations.

### Example:
```java
@Modifying
@Query("DELETE FROM User u WHERE u.id = :id")
void deleteUser(@Param("id") Long id);
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 10. How do you implement pagination and sorting in a Spring Boot application?
### Pagination:
```java
Page<User> findAll(Pageable pageable);
```

### Sorting:
```java
List<User> findAll(Sort sort);
```

### Example:
```java
Pageable pageable = PageRequest.of(0, 10, Sort.by("name").ascending());
Page<User> users = userRepository.findAll(pageable);
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 11. What is the N+1 selects problem in JPA, and how do you solve it in Spring Boot?
### Problem:
Occurs when an application executes N+1 SQL queries to fetch related entities.

### Solution:
1. **Fetch Joins**:
```java
@Query("SELECT u FROM User u JOIN FETCH u.posts")
List<User> findAllUsersWithPosts();
```

2. **Entity Graphs**:
```java
@Entity
@NamedEntityGraph(name = "User.posts", attributeNodes = @NamedAttributeNode("posts"))
public class User { ... }

@Query("SELECT u FROM User u")
@EntityGraph(value = "User.posts")
List<User> findAllUsersWithPosts();
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 12. How do you manage database connections in a Spring Boot application?
### Connection Pooling:
Spring Boot uses HikariCP by default.

### Configuration:
```properties
spring.datasource.hikari.maximum-pool-size=10
spring.datasource.hikari.minimum-idle=5
```

### Example:
```java
@Configuration
public class DataSourceConfig {
    @Bean
    @ConfigurationProperties("spring.datasource")
    public DataSource dataSource() {
        return DataSourceBuilder.create().build();
    }
}
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 13. What is the difference between eager and lazy fetching in JPA?
### Eager Fetching:
Fetches related entities immediately.

### Lazy Fetching:
Fetches related entities on demand.

### Example:
```java
@OneToMany(fetch = FetchType.LAZY)
private List<Post> posts;
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 14. How do you handle optimistic locking in JPA?
### Usage:
Use `@Version` annotation to handle versions.

### Example:
```java
@Entity
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    @Version
    private int version;

    private String name;
    // getters and setters
}
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---

### 15. What are some best practices for designing and maintaining Spring Data JPA repositories?
### Best Practices:
1. **Keep Repositories Clean**: Focus on data access operations.
2. **Use DTOs**: Avoid returning entities directly.
3. **Pagination and Sorting**: Always use pagination for large datasets.
4. **Custom Queries**: Use JPQL or native queries when necessary.
5. **Auditing**: Implement auditing for tracking changes.

### Example:
```java
public interface UserRepository extends JpaRepository<User, Long> {
    List<User> findByName(String name);
}
```
#### **[⬆ Back to Top](#spring-boot-data-access)**
---