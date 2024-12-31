# JWT Authentication with MongoDB

This project implements a signup and login flow using JWT (JSON Web Tokens) for authentication. It connects to a MongoDB database to manage user roles and user data.

## Requirements

To run this project, you will need to set up a MongoDB cluster and configure the application. Follow the steps below:

1. **Create a Free Cloud MongoDB Cluster:**
   - Go to [MongoDB Atlas](https://cloud.mongodb.com/).
   - Create a free cloud cluster.
   - Obtain your MongoDB connection string and replace the placeholder in the `application.properties` file.

2. **Create the Database and Collections:**
   - Create a database for the project (e.g., `mydb`).
   - Inside this database, create two collections: `roles` and `users`.

3. **Insert Initial Documents into the `roles` Collection:**
   - Insert the following documents into the `roles` collection:
     ```json
     {"name":"ROLE_USER"}
     {"name":"ROLE_ADMIN"}
     {"name":"ROLE_MODERATOR"}
     ```

## Running the Project

To run this project, use the following commands in your terminal or command prompt:
```bash
mvn install
mvn spring-boot:run
