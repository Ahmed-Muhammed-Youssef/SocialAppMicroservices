# **SocialApp Microservices**

Welcome to the **SocialApp Microservices** project!
This project is a modernized version of a monolithic social app, rearchitected using microservices for better scalability, maintainability, and flexibility. The goal is to showcase a clean, modular design with domain-focused boundaries, allowing for future expansions.

---

## **Table of Contents**
1. [About the Project](#about-the-project)
2. [Microservices Overview](#microservices-overview)
3. [Architecture](#architecture)
4. [Technologies Used](#technologies-used)

---

## **About the Project**

This project is a transformation of an older social app into a microservices architecture. The app allows users to connect, communicate, and share content seamlessly. By breaking down the monolith, the system achieves:
- **Scalability**: Services can scale independently.
- **Maintainability**: Each service can be developed, deployed, and maintained separately.
- **Flexibility**: Easy to add new features or services in the future.

---

## **Microservices Overview**

The application is divided into several key services:

1. **User Management**:
   - Handles user authentication, authorization, and profile management.
   - Includes secure signup, login, and profile updates.

2. **Newsfeed**:
   - Provides personalized content feeds for users.
   - Handles interactions like likes, comments, and shares.

3. **Messaging**:
   - Real-time chat functionality for user-to-user messaging.
   - Supports message delivery statuses and chat history.

4. **Content Management**:
   - Manages user-generated content, including posts, images, and media uploads.
   - Handles content moderation and storage.

Each service communicates using APIs or asynchronous messaging (e.g., RabbitMQ, Kafka) to ensure loose coupling.

---

## **Architecture**

This project follows a **microservices architecture** with a focus on clean, domain-driven design. The key components are:
- **APIs**: Each service exposes RESTful APIs for external and inter-service communication.
- **Database Per Service**: Each service owns its database, ensuring data independence.
- **Service Discovery**: Enables seamless communication between services.
- **Message Queue**: Used for asynchronous operations and event-driven workflows.

---

## **Technologies Used**

- **Backend**:
  - ASP.NET Core (C#)
  - Entity Framework Core (for data management)
  - SignalR (for real-time messaging)
- **Databases**:
  - SQL Server (User Management, Content Management)
  - MongoDB (Newsfeed, Messaging)
- **Communication**:
  - REST APIs
  - RabbitMQ (for messaging between services)
- **Authentication**:
  - IdentityServer or JWT-based authentication.
- **Containerization**:
  - Docker for containerizing services.
- **Orchestration**:
  - Docker Compose for service orchestration.
