# Microservices Order Management (Minimal Working Services)

This repository contains **4 independent minimal Spring Boot microservices**:

- order-service
- inventory-service
- payment-service
- notification-service

Each service can be run individually.

## How to run a service

```bash
cd order-service
mvn spring-boot:run
```

Then open the health endpoint:

```text
http://localhost:9000/api/health        # order-service
http://localhost:9001/api/health        # inventory-service
http://localhost:9002/api/health        # payment-service
http://localhost:9003/api/health        # notification-service
```
