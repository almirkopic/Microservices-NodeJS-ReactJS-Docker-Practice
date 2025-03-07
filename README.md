# Microservices-Based Application with Node.js, React, and Docker 🚀  

## 📖 Overview  
This project is a **microservices-based application** built with **Node.js** for the backend and **React** for the frontend. It follows an event-driven architecture where independent microservices communicate through an **event bus**, ensuring scalability and flexibility.  

## 📌 Project Structure  
The application consists of multiple microservices, each handling a specific responsibility:  

### 🏗️ Microservices  
- **Client** – React frontend for user interaction.  
- **Posts** – Handles post creation and storage.  
- **Comments** – Manages user comments on posts.  
- **Moderation** – Ensures comments follow rules before being published.  
- **Query** – Aggregates and structures data for the frontend.  
- **Event Bus** – Central service that facilitates communication between microservices.  

## 🔄 Workflow  
1. Users create **posts** via the **client**.  
2. Users can **comment** on posts.  
3. Comments are sent to the **moderation** service for approval.  
4. The **event bus** distributes events among microservices.  
5. The **query** service organizes data efficiently for frontend consumption.  

## 🚀 Getting Started  

### 1️⃣ Install Dependencies  
To set up the application, install dependencies in each microservice:  

```bash
cd client && npm i
cd ../comments && npm i
cd ../event-bus && npm i
cd ../moderation && npm i
cd ../posts && npm i
cd ../query && npm i
