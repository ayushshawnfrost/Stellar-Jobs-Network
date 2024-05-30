# Stellar-Jobs-Network

(Please head over to master branch for the code)

## Overview

This project is a comprehensive Spring Boot 3.x application that demonstrates the implementation of microservices architecture. It comprises three main microservices: Company, Jobs, and Reviews. The Company microservice publishes job listings, which are reviewed by the employees of those companies. The application leverages Eureka for service discovery, RabbitMQ for asynchronous inter-service communication, and an API Gateway for routing. Configuration management is handled by a Config Server. The database used is PostgreSQL, and the entire application is containerized using Docker and deployed on Kubernetes. For distributed tracing, Zipkin is used to track and monitor the communication between microservices.

## Microservices

### Company Microservice
- **Description:** Manages company details and job postings.

### Jobs Microservice
- **Description:** Manages job listings and their details.

### Reviews Microservice
- **Description:** Manages reviews for jobs posted by companies.

## Key Features

### Service Discovery
- **Eureka Clients:** All microservices are registered with Eureka, enabling service discovery and providing details about their health status.

### Asynchronous Communication
- **RabbitMQ:** Used for asynchronous communication between microservices, ensuring decoupling and reliability in message passing.

### API Gateway
- **Spring Cloud Gateway:** Routes incoming requests to the appropriate microservices and handles cross-cutting concerns such as security and rate limiting.

### Configuration Management
- **Config Server:** Centralized configuration management for all microservices, allowing dynamic configuration changes without redeployment.

### Database
- **PostgreSQL:** A robust relational database used for persisting data across all microservices.

### Containerization and Deployment
- **Docker:** Each microservice is containerized using Docker, ensuring consistent environments across development, testing, and production.
- **Kubernetes:** Manages the deployment, scaling, and orchestration of Docker containers, providing high availability and scalability.

### Distributed Tracing
- **Zipkin:** Used to trace and monitor the communication between microservices, providing insights into the performance and behavior of the system.


## Setup and Deployment

### Prerequisites
- Java 11 or higher
- Maven
- Docker
- Kubernetes (Minikube for local development)
- RabbitMQ
- PostgreSQL
