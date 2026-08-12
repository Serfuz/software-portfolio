# Board Game Café - Reservation & Management System

## Overview
This full-stack web application was developed by a six-person team as part of the University of Stavanger Software Engineering course (DAT240). The project received the highest grade (A). It supports board game management, user roles, table reservations, notifications, and payment workflows, and was implemented as a modular monolith using Domain-Driven Design and Vertical Slice Architecture.

## Technologies
- C#
- .NET
- React
- TypeScript
- PostgreSQL
- Entity Framework
- Docker
- GitHub Actions
- JWT authentication
- MediatR

## Team Size
- 6 computer engineering students

## My Contributions
- Helped shape the project’s architectural direction and early domain design, including the modular monolith structure and feature-based organization used across the application.
- Developed and maintained key parts of the Game Catalog Management domain, including the administration of games and game copies.
- Contributed to the admin-side experience by supporting dashboard functionality and operational features used to manage catalog content and application workflows.
- Worked on authentication and authorization flows to ensure the correct access rules for different user roles and protected application areas.
- Supported backend persistence work through PostgreSQL, Entity Framework, migrations, and data seeding efforts to keep the system stable and consistent.
- Helped resolve functional issues related to authorization, game-copy logic, and data integrity during integration and refinement stages.
- Acted as Product Owner for the project, helping maintain branch stability, review merge activity, and keep the team aligned on delivery priorities.

## What I Learned
- Domain-Driven Design
- Vertical Slice Architecture
- Event-driven communication
- Team-scale Git workflows
- CI/CD practices

## Project Overview

### Implemented Features
- User authentication and authorization for customers, stewards, and admins, including JWT-based login, protected routes, and forced password-change flows for first-time access.
- Game catalog management, including creating, viewing, editing, and removing board games, as well as game-copy tracking and rating/review support.
- Reservation lifecycle management, including creating reservations, checking availability, editing details, assigning tables, seating guests, handling no-shows, and canceling reservations.
- Payment workflows, including pricing calculation based on party size and duration, invoice requests, payment status tracking, and cafe payment handling.
- A notification system using SignalR and email workflows to inform users about reservation, payment, account, and password-related events.
- Cafe floor and table management, including customer-facing floor planning and steward tooling for reservation oversight and service operations.
- Admin and steward dashboard functionality for user management, policy configuration, and operational monitoring of the board game café.

### Architecture and Structure
- The backend is organized as a modular monolith using .NET, with distinct bounded contexts such as Account Management, Game Catalog Management, Reservation Management, Payment, Notifications, and Cafe Floor Management.
- Each feature area is separated into domain, application, infrastructure, and endpoint layers, following a Vertical Slice and Domain-Driven Design approach.
- Data access is handled through multiple Entity Framework DbContexts connected to a shared PostgreSQL database, with separate schemas and migrations for each area.
- Application behavior is coordinated through MediatR commands, queries, and domain events, enabling clear business workflows and integration between contexts.
- Validation, logging, and authorization are managed centrally in the API startup configuration, with FluentValidation and custom authorization policies enforcing business rules.
- The frontend is built with React and TypeScript, with route-based pages for customers, stewards, and administrators, along with shared authentication and notification components.
- Docker and Docker Compose are used to run the full stack consistently, including the frontend, backend, and supporting services.

### What this project Demonstrates
- A realistic full-stack software engineering workflow, from requirement-driven design to implementation, testing, and deployment.
- How a modular monolith can scale cleanly for a business domain without the overhead of a microservice architecture.
- Strong separation of concerns between business logic, persistence, API endpoints, and UI layers.
- Event-driven integration between domain areas such as reservations, payments, and notifications, showing how multiple features can remain decoupled while still working together.
- Best practices in team collaboration, Git workflow discipline, code organization, and CI/CD-oriented project structure.
- The practical use of modern web and backend technologies in a complete application that mirrors a real-world hospitality or venue management system.

