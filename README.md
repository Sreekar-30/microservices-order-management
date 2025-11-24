Microservices Order Management System

A modular Spring Boot Microservices project built to understand distributed systems, service isolation, and inter-service communication.
Each service runs independently with its own port and can be scaled or extended separately.

Tech Stack
| Layer        | Technology    |
| ------------ | ------------- |
| Language     | Java 17       |
| Framework    | Spring Boot 3 |
| Build Tool   | Maven         |
| Architecture | Microservices |
| IDE          | IntelliJ IDEA |

Services Included
This project contains four independent Spring Boot microservices:
order-service         → Port 9000
inventory-service     → Port 9001
payment-service       → Port 9002
notification-service  → Port 9003

Each service has:

Its own pom.xml
Its own src/main/java/...
Independent controller and main application file
Separate application.properties
Runs standalone


How to Run Each Service
Order Service
cd order-service
mvn spring-boot:run
Health: http://localhost:9000/api/health


Inventory Service
cd inventory-service
mvn spring-boot:run
Health: http://localhost:9001/api/health


Payment Service
cd payment-service
mvn spring-boot:run
Health: http://localhost:9002/api/health


Notification Service
cd notification-service
mvn spring-boot:run
Health: http://lo


Project Structure
microservices-order-management/
│── order-service/
│── inventory-service/
│── payment-service/
│── notification-service/
└── README.mdcalhost:9003/api/health


Every service contains:

src/
 └─ main/
     ├─ java/
     └─ resources/
pom.xml


Current Functionality

All services run independently
Dedicated ports for each microservice
Health check endpoints working
Clean, scalable folder structure
Ready for real microservice integration


Planned Enhancements

Service-to-service REST communication
Order → Inventory → Payment workflow
Database support for orders and stock
Notification trigger after order success
API Gateway (Spring Cloud Gateway)
Docker and Docker Compose support



Purpose of This Project

This project is part of my backend engineering practice.
I am building it to understand:
Microservice lifecycle
Independent deployment
Service isolation
Port managemen
Scalable backend architecture
