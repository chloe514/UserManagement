User Management Application
This is a simple User Management Application built with Spring Boot and Spring Security. It lets you manage users with different roles and provides secure authentication.

Features
Login with ADMIN and USER roles.
Secure password storage using BCrypt encryption.
Role-based access control—some endpoints are public, while others need you to log in.
What You Need
Make sure you have these installed:

Java 17 or higher
Maven (for building the project)
IntelliJ IDEA or any other Java-friendly IDE
Postman (optional, for testing APIs)
How to Set Up and Run
Clone the Project: First, get the project on your computer:

bash
Copy code
git clone https://github.com/yourusername/usermanagement.git
cd usermanagement
Build the Project: Use Maven to build the app. In the project folder, run:

bash
Copy code
mvn clean install
Run the Application: You can run the app using IntelliJ or through the command line:

bash
Copy code
mvn spring-boot:run
Test the Endpoints: Open your browser or Postman and try out these endpoints:

Endpoints
Public (no login needed):

URL: http://localhost:8080/greeting
Method: GET
Admin Only:

URL: http://localhost:8080/api/users
Method: GET
Login Details:
Username: admin
Password: admin
Other Authenticated Endpoints:

Just log in with the right credentials (admin or user) and try accessing other protected endpoints.
Login Details
Admin User:

Username: admin
Password: admin
Role: ADMIN
Regular User:

Username: user
Password: password
Role: USER
Common Errors and Fixes
404 Not Found: Double-check the URL; make sure it matches the endpoint.
401 Unauthorized: Check if the username and password are correct.
403 Forbidden: You’re logged in, but you don’t have the right role for this endpoint.