# GuestHouse Infrastructure

This repository contains the central orchestration files for running the entire **GuestHouse Microservices Architecture** using Docker Compose.

## Architecture Overview
The system consists of 3 independent Java Spring Boot microservices, each with its own dedicated MySQL database:
1. **Booking Service** (Port 8080) + Booking Database (`guesthousebooking`)
2. **Customer Service** (Port 8081) + Customer Database (`customerservice`)
3. **Review Service** (Port 8082) + Review Database (`reviewservice`)

## Required Repository Structure
For Docker Compose to build and link all services correctly, ensure that this infrastructure repository and all three service repositories are placed in the same parent folder:

```text
📁 parent-folder/
├── 📁 GuestHouse-Infrastructure/  (contains this docker-compose.yml)
├── 📁 GuestHouse-Booking-System/
├── 📁 GuestHouse-Customer-Service/
└── 📁 GuestHouse-Review-Service/
