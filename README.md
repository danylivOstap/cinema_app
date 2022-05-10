# Welcome to Cinema-App
## <a name="description"></a>Description
Simple WEB application that supports registration, authentication and CRUD operations.

## <a name="endpoints"></a>Endpoints:
* ``/inject`` - POST - Injects 2 new users into the database. Permission: Everyone.
* ``/register`` - POST - Register new user. Permission: Everyone.
* ``/login`` - POST - Login user. Permission: Everyone.
* ``/logout`` - POST - Logout user. Permission: Authenticated.
* ``/movies`` - GET - Get all movies. Permission: USER, ADMIN.
* ``/movie-sessions/available?movieId=<movieId>&date=<date>`` - GET - Get available movie sessions. Permission: USER, ADMIN.
* ``/cinema-halls`` - GET - Get all cinema halls. Permission: USER, ADMIN.
* ``/users/by-email?email=<email>`` - GET - Get user by email. Permission: ADMIN.
* ``/cinema-halls`` - POST - Create new cinema hall. Permission: ADMIN.
* ``/movies`` - POST - Create new movie. Permission: ADMIN.
* ``/movie-sessions`` - POST - Create new movie session. Permission: ADMIN.
* ``/orders/complete`` - POST - Complete order. Permission: USER.
* ``/movie-sessions/{id}`` - PUT - Update movie session. Permission: ADMIN.
* ``/movie-sessions/{id}`` - DELETE - Delete movie session. Permission: ADMIN.
* ``/shopping-carts/movie-sessions`` - PUT - Add movie session to shopping cart. Permission: USER.

---
## <a name="architecture"></a>3-layer architecture
1. DAO - Data access layer
2. Service - Application logic layer
3. Controllers - Presentation layer

---
## <a name="technologies"></a>Used Technologies:
* Java 11
* Apache Maven
* Apache Tomcat 9.0.50
* MySQL
* Spring Core
* Spring MVC
* Spring Security
* Hibernate

---
## <a name="start"></a>How to run a project?
1. Install MySQL and Apache Tomcat version 9.
2. Configure Apache Tomcat for your IDE.
3. Configure db.properties with your URL, USERNAME, PASSWORD, JDBC_DRIVER.
---