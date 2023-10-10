# Sample To Do List web application using Spring Boot and MySQL

A simple Todo list application using Spring Boot with the following options:

- Spring JPA and MySQL for data persistence
- Thymeleaf template for the rendering.

To build and run the sample from a fresh clone of this repo:

## Configure MySQL

Mysql is configured in `src/main/resources/application.properties` with environnement variable (`MYSQL_ADDON_DB...`), so if you use a mysql addon on clever cloud you only need to link your app with the database addon :)

N.B. We use Mysql 8.0 in this example

## Build and run the sample

You will need few variable on clevercloud application:

```bash
CC_CACHE_DEPENDENCIES="true"
CC_JAR_PATH="target/todo-0.0.1-SNAPSHOT.war"
CC_JAVA_VERSION="11"
```

Do not forget to link your application and your addon

As you add and update tasks in the app you can verify the changes in the database through the MySQL console using simple statements like 
`select * from todo_item`.


