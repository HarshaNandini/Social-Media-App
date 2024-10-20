# Harsha's Social Media App

A full-stack social media app built with Spring Boot and React. This project allows users to share posts, comment on posts, and manage profiles, showcasing a simple and scalable architecture.

## Table of Contents

- [Tech Stack](#tech-stack)
- [Features](#features)
- [Getting Started](#getting-started)
- [API Usage](#api-usage)

## Tech Stack

- **Frontend:** React, Chakra UI (for design components)
- **Backend:** Java, Spring Boot (for REST APIs), PostgreSQL (for database)

## Features

- User registration and authentication
- Create, read, update, and delete posts
- Add comments to posts
- View and update user profiles
- Responsive design with Chakra UI

## Getting Started

Follow these steps to get the app running locally.

### Prerequisites

Make sure you have the following installed:
- **Node.js** (for the React frontend)
- **Java** (for the Spring Boot backend)
- **PostgreSQL** (for the database)

### Backend Setup (Spring Boot)

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/social-media-app
   cd social-media-app/backend
   ```

2. **Configure the database:**
   Open `application.properties` in the `src/main/resources` folder and configure your PostgreSQL connection:
   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/your-database
   spring.datasource.username=your-username
   spring.datasource.password=your-password
   ```

3. **Build and run the backend:**
   ```bash
   ./mvnw spring-boot:run
   ```

   The backend will run at `http://localhost:8080`.

### Frontend Setup (React)

1. **Navigate to the frontend folder:**
   ```bash
   cd ../frontend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Run the frontend:**
   ```bash
   npm start
   ```

   The frontend will run at `http://localhost:3000`.

### Database Setup

1. **Create the database:**
   In PostgreSQL, create a database for your app:
   ```sql
   CREATE DATABASE social_media_db;
   ```

2. **Migrate tables:**
   The app will automatically set up tables when you start the backend.

## API Usage

After starting the backend, you can make API requests to interact with the app. Here's how you can use the API endpoints:

### Sample Requests:

1. **List all posts:**
   ```bash
   GET https://localhost:8080/api/posts/getall
   ```

2. **List comments by post:**
   ```bash
   GET https://localhost:8080/api/comments/getallbypost/{postId}
   ```

3. **User registration:**
   ```bash
   POST https://localhost:8080/api/auth/register
   ```

For more API details, refer to the Java controller classes in the `backend/src/main/java/com/yourapp/controllers` folder.
