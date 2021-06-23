# Employee-SpringBoot

Tasks:-
------
1.Create a spring boot rest service to store and retrieve data from MySQL database.
2.The service should be accessible only using basic authentication.
3.Create swagger config to validate and test the API.

Project Explanation:-
--------------------
  I.We can implement the following dependencies in the pom.xml file:-
  ------------------------------------------------------------------
   1.spring-boot-starter-parent
   ----------------------------
           -> The spring-boot-starter-parent is a project starter.
           ->  It provides default configurations for our applications.

   2.spring-boot-starter-actuator
  -------------------------------
            -> spring boot actuator is help us to monitor and manage the Spring Boot application.

  3.spring-boot-starter-data-jpa
  ------------------------------
             -> spring data JPA handles complexity of JDBC-based database access and ORM
             -> It reduces the boilerplate code by JPA.

  4.spring-boot-starter-web
  -------------------------
               -> spring-boot-starter-web related to web development.

  5.spring-boot-starter-validation
  -------------------------------
                -> it is Java Bean Validation with Hibernate Validator.  

  6.spring-boot-devtools
  ----------------------
                  -> If you any changes in code we don't restart the application. It will automatically restart.
                  -> It is also using to saving times for developers.

  7.mysql-connector-java
  ----------------------
                   -> It is provides database connectivity(JDBC) for client applications.

   II.Explain the java files in my project:-
   ----------------------------------------
    1.com.employee.controller:-

             EmployeeController.java -->It takes care of mapping request data to the defined request handler method.
    
    2.com.employee.model:-
        
             EmployeeInfo.java --> It is a POJO or Entity Class.
   
    3.com.employee.repository:-

              EmployeeRepository --> It contains the API for basic CRUD operations.

    4.com.employee.service:-

              EmployeeService --> It handles all the business logic by repository.

    5.com.employee.swaggerconfig:-

       --> It provides the OpenAPI Specification for creating RESTful API documentation formatted in JSON or YAML.
       --> springfox dependency provides Swagger 2 and Swagger UI.

   III.apllication.properties:-
   ---------------------------
       --> It is  built-in mechanism for application configuration using a file called application.properties
       --> It is located inside the src/main/resources folder.

   IV. The Annotations are used in my project:-
   -------------------------------------------
     1.This Annotations used for Controller class:-
            @RestController
            @RequestMapping
            @PostMapping
            @GetMapping
            @DeleteMapping

      2.This Annotations used for Model (POJO) class:-
            @Entity
            @Id
            @Column
            @GeneratedValue
            @NotBlank

      3.This Annotations used for Repository class:- 
            @Repository

       4.This Annotations used for Service class:-
            @Service

       5.This Annotations used for SwaggerConfig class:-
             @EnableSwagger2
             @Bean











     
