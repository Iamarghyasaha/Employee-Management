This project implements an Employee Management System using Spring MVC framework. It provides functionalities to manage employee records, including adding, updating, deleting, and listing employees. Below is an overview of the controller and its features:

Controller Overview
The EmployeeController manages HTTP requests related to employee operations:

List Employees: Retrieves all employees from the database and displays them.

Endpoint: GET /employees/list
Description: Fetches employees from the database using EmployeeService and adds them to the model for rendering in the list-employees view.
Show Form for Adding an Employee: Displays a form to add a new employee.

Endpoint: GET /employees/showFormForAdd
Description: Initializes a new Employee object and adds it to the model for rendering in the employee-form view.
Save Employee: Processes the form submission to save a new or updated employee.

Endpoint: POST /employees/save
Description: Saves the employee using EmployeeService, redirects to the list of employees to prevent duplicate form submission.
Show Form for Updating an Employee: Displays a form populated with the details of a specific employee for updating.

Endpoint: GET /employees/showFormForUpdate
Parameters: employeeId (Employee ID)
Description: Fetches the employee by ID using EmployeeService and adds it to the model for rendering in the employee-form view.
Delete Employee: Deletes a specific employee by ID.

Endpoint: GET /employees/delete
Parameters: employeeId (Employee ID)
Description: Deletes the employee using EmployeeService and redirects to the list of employees.
Technologies Used
Spring MVC: Framework for building web applications in Java.
Spring Boot: Simplifies Spring application development.
Thymeleaf: Server-side Java template engine for web and standalone environments.
Maven: Build automation tool and dependency management.
MySQL: Relational database for storing employee data.
Getting Started
Prerequisites
Java 8 or higher installed on your machine.
Maven installed to build and run the application.
MySQL database server running locally or remotely.
Installation and Setup
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/employee-management.git
Navigate to the project directory:

bash
Copy code
cd employee-management
Build the project using Maven:

bash
Copy code
mvn clean install
Configure MySQL database settings in application.properties file located in src/main/resources.

Run the application:

bash
Copy code
mvn spring-boot:run
Access the application in your web browser at http://localhost:8080.

Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

License
This project is not licensed; feel free to use it as you like!
