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

#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-core)**
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
#### **[⬆ Back to Top](#level--spring-boot-annotations)**
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
#### **[⬆ Back to Top](#level--spring-boot-annotations)**
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
#### **[⬆ Back to Top](#level--spring-boot-annotations)**
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
#### **[⬆ Back to Top](#level--spring-boot-annotations)**
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

#### **[⬆ Back to Top](#level--spring-boot-annotations)**
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
#### **[⬆ Back to Top](#level--spring-boot-annotations)**
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

#### **[⬆ Back to Top](#level--spring-boot-annotations)**
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
#### **[⬆ Back to Top](#level--spring-boot-annotations)**
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

#### **[⬆ Back to Top](#level--spring-boot-annotations)**
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
#### **[⬆ Back to Top](#level--spring-boot-annotations)**
---