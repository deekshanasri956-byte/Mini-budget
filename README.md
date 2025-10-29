MiniBudget+ – Smart Expense & Goal Tracker
Project Overview
MiniBudget+ is a full-stack web application designed to help users efficiently manage their personal finances.
It allows users to record, categorize, and monitor income and expenses in real time, while offering an interactive dashboard for visual financial insights and goal tracking.

⚙️ Tech Stack
Layer =	Technologies Used
Frontend =	React.js, HTML, CSS, JavaScript
Backend =	Spring Boot (Maven)
Database =	MySQL
Tools	= Eclipse (for backend), VS Code (for frontend), Postman (for API testing)

Key Features :
Add, edit, and delete income & expenses
Real-time expense visualization with charts
Set and track financial goals
Secure data storage using MySQL
RESTful API integration between backend and frontend
Voice-based expense logging (optional enhancement)

Project Structure:
MiniBudgetPlus/
│
├── minibudget-frontend/     # React Frontend (VS Code)
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── minibudget-backend/      # Spring Boot Backend (Eclipse)
│   ├── src/main/java/
│   ├── src/main/resources/
│   ├── pom.xml
│   └── ...
│
└── README.md
How to Run the Project:
Step 1️: Start the Backend (Eclipse)
1.Open Eclipse → Import the Spring Boot project (minibudget-backend).
2.Go to application.properties and verify:
server.port=8085
spring.datasource.url=jdbc:mysql://localhost:3306/minibudget
spring.datasource.username=root
spring.datasource.password=yourpassword
3.Run the application:
mvn spring-boot:run
4.Backend will start at: http://localhost:8085
Step 2️: Start the Frontend (VS Code)
1.Open VS Code → Navigate to the frontend folder:
-cd minibudget-frontend
2.Install dependencies:
-npm install
3.Start the frontend:
-npm start
4.Frontend runs on: http://localhost:3000
Step 3️: Connect Frontend and Backend
In your React app’s .env or API file:
-const BASE_URL = "http://localhost:8085/api";

Future Enhancements:
- Expense alerts and reminders
- Mobile-friendly version
- Cloud-based backup
- Export reports as PDF/Excel
