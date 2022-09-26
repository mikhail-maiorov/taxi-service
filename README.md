# :taxi:   taxi-service   :taxi:

## :key:  About

This web application represents a simple version of a taxi service. 

## :mag:  Details

Using this application you can:
- add a driver/manufacturer/car to the database 
- update driver's data
- delete the driver/manufacturer/car
- get information about the driver/car/manufacturer
- login and logout

## :scroll:  Project Structure

In this project used the n-tire architecture

- DAO tire - allows to modify data in database using CRUD methods
- Service tire - this is where all the logic happens
- Controller tire - provides an interface to interact with application

## :hammer_and_wrench:  Technologies

- Java 11
- JDBC
- Apache Maven 3.8.0
- Java Servlet API
- JSP
- MySQL 8.0.30
- Apache Tomcat 9.0.50

## :gear:  How to launch

- Fork this project to your repository
- Clone it to your PC and open it in IDE
- Create a database using init_db.sql ("/resources" folder)
- Edit the ConnectionUtil class to add custom settings:
```java
    private static final String URL = "URL_TO_YOUR_DATABASE";
    private static final String USERNAME = "YOUR_DATABASE_USERNAME";
    private static final String PASSWORD = "YOUR_DATABASE_PASSWORD";
```
- Download and extract [Tomcat 9.0.50](https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.50/bin/)
- Change the configuration to use "Tomcat Server Local": 
  - in Intellij IDEA: Run -> Edit Configurations... -> "+" -> Tomcat Server -> Local
  - in Server tab: in Application Server click Configuration and find the Tomcat folder
  - click the "fix" button at the bottom
  - click the "taxi-service:war exploded"
  - delete the line in the "Application context" field
  - click OK
- Run the project :rocket:
