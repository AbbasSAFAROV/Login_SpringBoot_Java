# Login_SpringBoot_Java

https://start.spring.io/

### Technologies

-Maven

-Language: Java

-Spring Boot: 2.6.1

-Java: 11

### Dependencies

Spring Web(Web)

Spring Data JPA(SQL)

Thymeleaf(Template Engines)

MySQL Driver(SQL)

Spring Security(Security)

Spring Boot DevTools(Developer Tools)


![image](https://user-images.githubusercontent.com/61595808/144246763-0137ed1f-8396-4921-ba08-78a87309d3e4.png)


### How can I connect to the database?

Which Database you will use, you must enter the information about it.  ---> application.properties

after my codes :

Hibernate: create table role (id bigint not null auto_increment, name varchar(255), primary key (id)) engine=InnoDB
Hibernate: create table user (id bigint not null auto_increment, email varchar(255), first_name varchar(255), last_name varchar(255), password varchar(255), primary key (id)) engine=InnoDB
Hibernate: create table users_roles (user_id bigint not null, role_id bigint not null) engine=InnoDB

![image](https://user-images.githubusercontent.com/61595808/144304433-861ad952-83df-419f-9bf9-c5f5f21f9552.png)







