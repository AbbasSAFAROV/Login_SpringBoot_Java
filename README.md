# Login_SpringBoot_Java

Youtube: https://www.youtube.com/watch?v=TGRPIKCrpQk

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


### My Database

My Datbase name is "try".I have 3 table.role,user,users_roles

![image](https://user-images.githubusercontent.com/61595808/144309982-0ef489b3-64d3-4e87-b398-0e6868dbe5b1.png)


### -role-

![image](https://user-images.githubusercontent.com/61595808/144310198-4f50793b-b4f6-4fbf-9010-c7c4f5f67abe.png)


### -user-

![image](https://user-images.githubusercontent.com/61595808/144310308-f5df235a-1e08-4802-8b4b-fe94287f9f3b.png)


### -users_roles-

![image](https://user-images.githubusercontent.com/61595808/144310415-d08032f5-6642-417e-9c20-377cc3cc51c5.png)



DTO:Data Transfer Object





Using generated security password: 5d22314e-24aa-442f-8c44-b1cacf8bbaa7

![image](https://user-images.githubusercontent.com/61595808/144587600-92c83dfd-1c84-4942-83cc-ea14a9d2e30d.png)


### Error

I got this error.

![image](https://user-images.githubusercontent.com/61595808/144604005-8c69cfcd-b733-45bd-80a4-9c8c65e7da3d.png)

 @Autowired
 
    private BCryptPasswordEncoder passwordEncoder;

when I removed the "@Autowired" in this part it worked.

But the code did not save it to the database. And it still didn't work properly. When I added "@Lazy" it worked completely.

![image](https://user-images.githubusercontent.com/61595808/144708337-ed691c16-3163-4a6f-a8a9-c3df3067daed.png)

