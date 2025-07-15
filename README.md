# Number-Cruncher
🧮 Spring Boot Calculator API
A simple RESTful Calculator built with Spring Boot. This application provides basic arithmetic operations like addition, subtraction, multiplication, and division through HTTP GET endpoints.

📁 Project Structure
calculator/
├── .idea/                   # IntelliJ IDEA project files
├── .mvn/                    # Maven wrapper support files
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com.example.calculator/
│   │   │       ├── controller/
│   │   │       │   └── CalculatorController.java   # Handles REST API endpoints
│   │   │       ├── service/
│   │   │       │   └── CalculatorService.java      # Business logic for calculations
│   │   │       └── CalculatorApplication.java      # Main class to bootstrap Spring Boot
│   │   └── resources/
│   │       └── application.properties              # Configurations (currently empty)
│   └── test/                                       # Unit tests (optional)
├── target/                                         # Compiled classes and packaged .jar
├── .gitignore
├── pom.xml                                         # Maven build configuration
├── mvnw, mvnw.cmd                                  # Maven wrapper scripts
└── README.md                                       # Project documentation
🔧 Features
Addition: /api/calc/add?a=5&b=10

Subtraction: /api/calc/subtract?a=10&b=4

Multiplication: /api/calc/multiply?a=3&b=7

Division: /api/calc/divide?a=12&b=4

All endpoints use GET requests with @RequestParam parameters a and b.

▶️ How to Run
Clone the repository:

git clone https://github.com/your-username/spring-boot-calculator.git
cd spring-boot-calculator
Run using Maven wrapper:

./mvnw spring-boot:run
or if you're on Windows:

mvnw.cmd spring-boot:run
Access the API in browser or Postman:

http://localhost:8080/api/calc/add?a=10&b=5
http://localhost:8080/api/calc/sutract?a=10&b=5
http://localhost:8080/api/calc/multiply?a=10&b=5
http://localhost:8080/api/calc/divide?a=10&b=5
📦 Dependencies
Spring Boot Starter Web

Maven (wrapper included)

🤔 Why This Project?
This project was built as a learning exercise to:

Understand Spring Boot architecture

Create RESTful services

Implement clean code structure with controller-service separation

Use Maven for project management

📌 Future Enhancements
Add input validation
Implement logging and exception handling
Create a frontend using HTML/React
Add unit and integration tests
