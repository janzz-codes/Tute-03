<<<<<<< HEAD
# OOP Tutorial 3 — Product Service

Module: 5COSC019C Object Oriented Programming

This project demonstrates a `Product` model, an in-memory `List<Product>`, a Spring `ProductService`, REST endpoints, Swagger UI, and a PlantUML class diagram.

## Requirements

- Java 17 or later
- Maven (or IntelliJ IDEA's bundled Maven)
- Internet access on the first Maven build to download dependencies

## Run in IntelliJ IDEA

1. Extract this ZIP file.
2. In IntelliJ, choose **File → Open** and select the extracted project folder containing `pom.xml`.
3. Allow Maven to load the dependencies.
4. Run `ProductsApiApplication.java`.
5. Open Swagger UI at `http://localhost:8080/swagger-ui/index.html`.

## Endpoints

| Method | URL | Purpose |
|---|---|---|
| GET | `/products` | Get all products |
| GET | `/products/{id}` | Get one product by ID |
| POST | `/products` | Add a product |
| DELETE | `/products/{id}` | Delete a product |
| GET | `/products/search?name=Lap` | Search names (additional guide activity) |

## Swagger test sequence

1. Use `POST /products` with this JSON body (do not send an ID):
   ```json
   {
     "name": "Laptop",
     "price": 899.99
   }
   ```
2. POST another product:
   ```json
   {
     "name": "Mouse",
     "price": 24.99
   }
   ```
3. Call `GET /products`. You should see both products, with IDs 1 and 2.
4. Call `GET /products/1`. It should return the laptop.
5. Call `DELETE /products/1`.
6. Call `GET /products` again. Only the mouse should remain.
7. Test `GET /products/search?name=Mou`.


=======
# Tute-03
Week 04 Tutorial 
>>>>>>> be303e0fd597a78af8887de12585f2645c346782
