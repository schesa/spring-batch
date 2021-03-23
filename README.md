# Spring batch demo

## Starting **Spring Cloud Data Flow**

Run start.bat

## Bill setup task

Is a simple Spring Cloud task.

Creates a table in the database.

In mysql.ps1 you can find a docker container setup for mysql.

To run standalone:

```
./mvnw package
./java-jar.bat
```

## Bill run

Is a Spring Batch app.

Processes /resources/usageinfo.json into rows in the table define in Bill setup task.

In mysql.ps1 you can find a docker container setup for mysql.

To run standalone:

```
./mvnw package
./java-jar.bat
```

## Spring

Is a Spring Boot scheduler app.

When started, starts a task every 3 seconds using Spring Cloud Data Flow Rest API

# Documentation

https://dataflow.spring.io/docs/batch-developer-guides/
