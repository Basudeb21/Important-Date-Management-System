# Intelligent Event & Reminder Management System (IERMS)

## Overview

IERMS (Intelligent Event & Reminder Management System) is a production-grade backend application built using Spring Boot.

The project is designed as a complete backend engineering practice system to learn and implement enterprise-level backend development concepts including:

* Spring Boot
* Spring Security
* JWT Authentication
* OAuth2 Login
* JPA & Hibernate
* Redis Caching
* Scheduling & Cron Jobs
* Docker & Deployment
* Testing
* API Documentation
* Microservice-ready architecture

This project is not just a CRUD application.
It is a full-scale backend learning and engineering project focused on real-world architecture and scalable backend development.

---

# Project Vision

The main goal of this project is to:

* Learn backend engineering deeply
* Understand enterprise architecture
* Build production-style REST APIs
* Practice scalable application structure
* Master Spring Security and JPA
* Prepare for real-world backend development
* Build a future microservice-ready system

---

# Tech Stack

## Backend

* Java 21
* Spring Boot 3
* Maven

## Database

* PostgreSQL

## Security

* Spring Security
* JWT Authentication
* OAuth2 Login

## Cache

* Redis

## API Documentation

* Swagger / OpenAPI

## Testing

* JUnit
* Mockito
* Postman

## DevOps

* Docker
* Docker Compose
* Kubernetes (Future)

---

# Current Development Phase

## Phase 1 — Foundation & Event CRUD

Currently implementing:

* Project setup
* Layered architecture
* REST APIs
* DTO mapping
* Validation
* Exception handling
* Event CRUD operations
* JPA entity relationships

---

# Planned Features

## Authentication Module

* User Registration
* Login
* JWT Authentication
* Refresh Token
* Logout
* Forgot Password
* Reset Password
* OAuth2 Login

## User Module

* Update Profile
* Change Password
* Delete Account
* Notification Preferences
* Timezone Settings

## Event Management Module

* Create Event
* Update Event
* Delete Event
* Archive Event
* Favorite Event
* Upcoming Events
* Today’s Events
* Monthly Events
* Recurring Events

## Reminder & Notification Module

* Scheduled Reminders
* Email Notifications
* Daily Summary
* Notification History
* Read/Unread Tracking

## AI Integration Module

* AI-generated wishes
* Smart reminder text
* Greeting generation
* Emotional/funny/professional wishes

## Dashboard & Analytics Module

* Event statistics
* Category analytics
* Monthly reports
* Upcoming reminders count

## Redis Cache Module

* Dashboard caching
* User profile caching
* Analytics caching
* Upcoming events caching

## Search & Filter Module

* Search by title
* Search by category
* Search by date
* Sorting
* Pagination

---

# Core Learning Topics Covered

## Spring Boot

* IOC Container
* Dependency Injection
* Bean Lifecycle
* Auto Configuration
* MVC Architecture
* REST APIs

## JPA & Hibernate

* Entity Relationships
* JPQL
* Native Queries
* Pagination
* Projection
* Transactions
* Dirty Checking
* Cascading
* orphanRemoval
* FetchType.LAZY/EAGER
* N+1 Optimization

## Spring Security

* JWT Authentication
* OAuth2 Login
* Role-based Authorization
* Method-Level Security
* Security Filter Chain

## Redis

* CacheManager
* @Cacheable
* @CacheEvict
* Redis Configuration

## Scheduler

* @Scheduled
* Cron Expressions
* Background Jobs

## Testing

* Unit Testing
* Integration Testing
* Mocking with Mockito

## DevOps

* Docker
* Docker Compose
* Kubernetes Basics
* Deployment

---

# Project Structure

```text
src/main/java
├── config
├── controller
├── dto
│   ├── request
│   └── response
├── entity
├── enums
├── exception
├── mapper
├── repository
├── security
├── service
│   ├── impl
│   └── interfaces
├── scheduler
├── notification
├── ai
├── cache
├── analytics
├── validation
├── util
└── common
```

---

# Initial API Endpoints

## Event APIs

```http
POST   /api/events
GET    /api/events
GET    /api/events/{id}
PUT    /api/events/{id}
DELETE /api/events/{id}
```

---

# Database Tables (Planned)

## USERS

| Column     | Type      |
| ---------- | --------- |
| id         | BIGINT    |
| name       | VARCHAR   |
| email      | VARCHAR   |
| password   | VARCHAR   |
| role       | VARCHAR   |
| provider   | VARCHAR   |
| created_at | TIMESTAMP |

## EVENTS

| Column        | Type      |
| ------------- | --------- |
| id            | BIGINT    |
| title         | VARCHAR   |
| description   | TEXT      |
| event_type    | VARCHAR   |
| event_date    | DATE      |
| reminder_time | TIMESTAMP |
| priority      | VARCHAR   |
| recurring     | BOOLEAN   |
| archived      | BOOLEAN   |
| favorite      | BOOLEAN   |
| user_id       | BIGINT    |

## NOTIFICATIONS

| Column      | Type      |
| ----------- | --------- |
| id          | BIGINT    |
| message     | TEXT      |
| read_status | BOOLEAN   |
| event_id    | BIGINT    |
| created_at  | TIMESTAMP |

---

# Development Roadmap

## Phase 1

* Spring Boot Foundation
* CRUD APIs
* Layered Architecture

## Phase 2

* JPA Relationships
* JPQL
* Pagination
* Projections

## Phase 3

* Spring Security
* JWT Authentication
* OAuth2 Login
* Roles & Permissions

## Phase 4

* Validation
* Exception Handling

## Phase 5

* Scheduler
* Email System

## Phase 6

* Redis Caching

## Phase 7

* Testing

## Phase 8

* Docker & Deployment

## Phase 9

* Kubernetes Basics

## Phase 10

* Microservice Conversion

---

# Future Microservices Architecture

Possible future services:

* Auth Service
* Event Service
* Notification Service
* AI Service
* User Service
* API Gateway

---

# Future Features

* WhatsApp Integration
* Telegram Bot
* Push Notifications
* Voice Assistant
* Mobile App
* Shared Family Calendar
* Team Collaboration
* AI Smart Assistant

---

# Setup Instructions

## Clone Repository

```bash
git clone <your-repository-url>
```

## Navigate to Project

```bash
cd ierms
```

## Run Application

```bash
./mvnw spring-boot:run
```

---

# Author

Developed as a backend engineering learning project focused on mastering Spring Boot ecosystem and enterprise backend development.

---

# Important Learning Rules

1. Implement feature-by-feature.
2. Understand every line of code.
3. Commit code regularly.
4. Focus on architecture and scalability.
5. Learn concepts deeply instead of copying tutorials.

---

# Status

🚧 Currently in active development.
