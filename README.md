# SIT737-2025-t1-prac5p
This repository contains a Dockerized Node.js Calculator Microservice for University unit SIT737, Task 5.1P. It supports basic arithmetic operations with input validation, logging via Winston, Docker Compose deployment, and health checks for container monitoring.

# 🚀 Features

1. Addition, subtraction, multiplication, and division operations
2. Input validation and error handling
3. Winston logging for requests and errors
4. Dockerized for easy deployment
5. Docker Compose setup with health check support

# 🛠️ Technologies Used

1. Node.js
2. Express.js
3. Winston (Logging)
4. Docker
5. Docker Compose

# 📂 Project Structure

SIT737-2025-T1-PRAC5P/
├── logs/
├── node_modules/
├── calculator.js
├── docker-compose.yml
├── Dockerfile
├── package.json
├── package-lock.json
└── README.md

# ⚙️ Getting Started

**Prerequisites**

1. Node.js
2. Docker
3. Git

# Installation

**Clone the repository:**

git clone https://github.com/DanishKumar1001/SIT737-2025-t1-prac5p.git
cd SIT737-2025-t1-prac5p

**Build the Docker image:**

docker build -t calculator-microservice .

**Run with Docker Compose:**

docker-compose up --build

**Access the application:**

http://localhost:3000

# 📈 API Endpoints

Method	     Endpoint	     Description	                          Example Usage

GET	          /add	        Adds two numbers	                    /add?num1=5&num2=3
GET	          /subtract     Subtracts second number from first  	/subtract?num1=10&num2=5
GET	          /multiply	    Multiplies two numbers          	    /multiply?num1=4&num2=3
GET	          /divide	    Divides first number by second	        /divide?num1=10&num2=2

# 🩺 Health Check

**Docker Compose includes a health check that:**

1. Tests if the application is reachable via curl
2. Restarts the container automatically if health check fails

# 🐳 Docker Commands Quick Reference

Reference : https://docs.docker.com/

**Build Image:**

docker build -t calculator-microservice .

**Run Container:**

docker run -p 3000:3000 calculator-microservice

**Docker Compose Up:**

docker-compose up --build

**Docker Compose Down:**

docker-compose down
