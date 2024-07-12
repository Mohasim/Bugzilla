# Bucktracker JPA Project

## Overview

The Bucktracker JPA project is a Java-based application designed for tracking bugs and managing releases. It utilizes Spring Boot for its framework and Hibernate for JPA implementation.

## Prerequisites

- Java JDK 8 or higher
- Maven for dependency management and project build
- An IDE like IntelliJ IDEA or Eclipse

## Libraries and Frameworks

This project includes the following main dependencies:

- Spring Web (`org.springframework:spring-web:5.0.5.RELEASE`)
- Hibernate Validator (`org.hibernate.validator:hibernate-validator:6.0.9.Final`)
- Tomcat Embed (`org.apache.tomcat.embed:tomcat-embed-core:8.5.29` and related)
- Javax Validation API (`javax.validation:validation-api:2.0.1.Final`)

For testing, the following libraries are used:

- AssertJ (`org.assertj:assertj-core:3.9.1`)
- Mockito (`org.mockito:mockito-core:2.15.0`)
- Byte Buddy (`net.bytebuddy:byte-buddy-agent:1.7.11`)
- Hamcrest (`org.hamcrest:hamcrest-core:1.3` and `org.hamcrest:hamcrest-library:1.3`)

## Project Structure

The project follows a standard Maven project structure with its source code located under `src/main/java` and resources under `src/main/resources`. Tests are located under `src/test/java`.

## Building the Project
The application uses an H2 In Memory database, with the console being found at http://localhost:8080/console
The jdbc url should be: jdbc:h2:mem:bugtracker
The user name is "sa" and there is no password

To build the project, navigate to the root directory and run:

```sh
./mvnw clean install
```

For Windows, use:

```sh
mvnw.cmd clean install
```

## Running the Application

After building, you can run the application using:

```sh
./mvnw spring-boot:run
```

Or for Windows:

```sh
mvnw.cmd spring-boot:run
```

## Contributing

Contributions are welcome. Please feel free to submit a pull request or open an issue for discussion.
