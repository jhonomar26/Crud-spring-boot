# Customer Management System  

## Project Description  
This is a customer management system developed using **Spring Boot**, **Spring Security**, **JPA**, and a relational database. It allows performing CRUD operations (Create, Read, Update, and Delete) on customers, with implemented validations and security features.  

## Key Features  
- ✅ Customer listing with detailed information  
- ✅ Add, edit, and delete customers  
- ✅ Form validations with Bootstrap and HTML5  
- ✅ Security management with Spring Security  
- ✅ Database connection using JPA  
- ✅ Responsive interface with Bootstrap  
- ✅ Multi-language support  

## Technologies Used  
- Java 17+  
- Spring Boot  
- Spring Security  
- JPA / Hibernate  
- Bootstrap  
- Thymeleaf  
- Relational database Mysql

## Installation & Setup  
### 🔹 **Prerequisites**  
Before running the project, make sure you have installed:  
✅ **Java 17+** (check with `java -version`)  
✅ **Maven** (check with `mvn -version`)  
✅ **MySQL** (or your chosen database)  
✅ **Git** (to clone the repository)  

### 🔹 **Database Configuration**  
- **Ensure that MySQL is running** and that the `test` database exists. If not, create it with:  
  ```sql
  CREATE DATABASE test;
  ```
- **Set your username and password** in `application.properties`:  
  ```properties
  spring.datasource.username=your_username
  spring.datasource.password=your_password
  ```

### 🔹 **Dependencies in `pom.xml`**  
Ensure that you have the necessary dependencies for **Spring Boot**, **Spring Security**, **JPA**, **Thymeleaf**, **Bootstrap**, and **MySQL Driver**.  

### 🔹 **Run the Project**  
1. Navigate to the project directory:  
   ```bash
   cd project-name
   ```  
2. Compile and run the project using Maven:  
   ```bash
   mvn spring-boot:run
   ```  
3. **Access the application** in your browser:  
   ```
   http://localhost:8080
   ```

### 🔹 **Additional Configurations**  
If you experience issues with Thymeleaf caching, make sure caching is disabled:  
```properties
spring.thymeleaf.cache=false
```
To **display SQL queries**, enable:  
```properties
logging.level.org.hibernate.SQL=DEBUG
logging.level.org.hibernate.orm.jdbc.bind=TRACE
```
If using **a different database (PostgreSQL, H2, etc.)**, update `spring.datasource.url` and the Hibernate dialect accordingly.  

### 🔹 **Users and Security**  
If authentication is required, ensure users and permissions are properly configured in **Spring Security**.  

With this setup, your project should run smoothly. 🚀
