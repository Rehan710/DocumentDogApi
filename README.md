# DocumentDogApi
 Dog REST API code documenting it using Swagger.

One of the most popular API documentation specifications is OpenApi, formerly known as the Swagger Specification. OpenAPI allows you to describe your API using JSON or YAML. 

Swagger is the name associated with some of the most well-known, and widely used tools for implementing the OpenAPI specification. Swagger helps you design, build, document and consume REST APIs. SpringFox is a Swagger integration for the Spring Framework.

Swagger Editor – A browser-based editor where you can write OpenAPI specs.
Swagger UI – A web application that renders OpenAPI specs as interactive API documentation.
Swagger Codegen – A tool that generates server stubs and client libraries from an OpenAPI spec.

The case study to be documented is a REST API that retrieves a list of locations from a database. 

The REST API has the following components:

Controller - DogController.java

Service - DogService.java and DogServiceImpl.java

CRUD Repository - DogRepository.java

Domain Entity/Model - Dog.java

Swagger Config - SwaggerConfig.java

H2 Database accessible via http://localhost:8080/h2/

Tomcat Server accessible via http://localhost:8080

Swagger UI via http://localhost:8080/swagger-ui.html



Step 1: Add the necessary dependencies for Swagger.



<dependency>
            <groupId>io.springfox</groupId>
            <artifactId>springfox-swagger-ui</artifactId>
            <version>2.9.2</version>
        </dependency>

        <dependency>
            <groupId>io.springfox</groupId>
            <artifactId>springfox-swagger2</artifactId>
            <version>2.9.2</version>
            <scope>compile</scope>
            </dependency>



Step 2: Configure Swagger using a Docket Bean.

Step 3: Utilize Swagger UI to review and test your API.
Now, you should be able to head to http://localhost:8080/swagger-ui.html#/ and test out your API.


If you click on one of the available commands for your API, you should be able to Try it out and test that it works correctly. Depending on which you test, you may need to provide information (such as the id for getBreedByID), or be able to immediately Execute the query.
