eCommerce API – Spring Boot & MySQL
Overview

This project is a beginner friendly RESTful eCommerce API built using Java, Spring Boot, and MySQL. It allows you to manage products, categories, users, orders, and shopping cart data for an online store.

The goal of this project was to learn how backend systems connect together, how controllers talk to the database using DAOs, and how to test API endpoints using Insomnia.

What This API Does

This API allows you to:

• Get a list of products
• Get a list of categories
• Search for products
• Manage shopping cart items
• Connect Java controllers to a MySQL database
• Return clean JSON responses

All data is stored in a MySQL database and accessed using DAO (Data Access Object) classes.

Project Structure (Simple Explanation)

This project follows a common Spring Boot structure:

Controllers

Controllers handle HTTP requests.
Example: when you go to /products, the ProductsController decides what happens.

DAO (Data Access Objects)

DAOs handle communication with the database.
They run SQL queries and return Java objects.

Models

Models represent database tables as Java classes.
Example: a Product model matches the products table in MySQL.

Database

MySQL stores all the data such as products, categories, and users.

What I Worked On
Fixing and Completing Controllers

I fixed and completed the ProductsController and CategoriesController by:

• Connecting them properly to their DAO classes
• Fixing broken logic that caused incorrect data to return
• Making sure endpoints returned JSON correctly

This helped me understand how Spring Boot connects controllers to the database layer.

Fixing a Database Bug (Duplicate Products)

While testing the API, I noticed duplicate products were appearing.

The problem was caused by:
• Using INSERT statements instead of UPDATE statements in SQL

How I fixed it:
• Reviewed the SQL scripts
• Identified duplicate product records
• Replaced incorrect INSERTs with UPDATE queries
• Verified duplicates were removed

After fixing this, products displayed correctly with no duplicates.

Testing with Insomnia

I used Insomnia to test all API endpoints.

What I learned:
• How to send GET requests to the API
• How to check JSON responses
• How to write after-response scripts
• How to test array lengths and returned data

Example test:
• Confirming the number of products returned
• Making sure search results work correctly

This helped ensure the API works as expected.

Technologies Used

• Java
• Spring Boot
• MySQL
• JDBC
• Insomnia
• REST APIs

How to Run the Project

Clone the repository

Open the project in IntelliJ

Run the SQL script to create the database

Update database credentials in application.properties

Run the Spring Boot application

Test endpoints using Insomnia

Example Endpoints

• GET /products – Get all products
• GET /categories – Get all categories
• GET /products?search= – Search for products

Responses are returned in JSON format.

What I Learned From This Project

• How Spring Boot controllers work
• How DAOs connect Java to MySQL
• How small SQL mistakes can cause big bugs
• How to debug backend issues step by step
• How to test APIs using Insomnia

Why This Project Matters

This project shows my ability to:

• Debug real backend issues
• Understand full-stack data flow
• Work with databases safely
• Test and validate APIs
• Learn and fix problems independently
