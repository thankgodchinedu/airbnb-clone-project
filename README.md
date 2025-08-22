# Airbnb Clone Project

## Overview
The Airbnb Clone Project is a real-world web application designed to simulate the functionality of a booking platform like Airbnb. It focuses on backend systems, database design, API development, and application security.

## Project Goals
- Master collaborative workflows using GitHub
- Deepen understanding of backend architecture & database design
- Implement security measures in API development
- Learn CI/CD pipelines for efficient deployment
- Document and plan complex Software projects
- Work with Django, MySQL, and GraphQL

## Tech Stack
- **Backend Framework**: Django (Python)
- **Database**: MySQL
- **API**: Django REST Framework & GraphQL
- **DevOps Tools**: Docker, GitHub Actions
- **Version Control**: Git & GitHub

## Team Roles  

In this project, we adopt standard software development team roles to ensure clarity, collaboration, and smooth delivery. Each role contributes uniquely to building the Airbnb Clone.  

### 1. Business Analyst (BA)  
Gathers and analyzes project requirements, ensuring the development team builds features that meet user and business needs.  

### 2. Product Owner (PO)  
Owns the product backlog and prioritizes features based on value and impact.  

### 3. Product Manager (PM)  
Defines the vision, strategy, and roadmap of the product, coordinating with all stakeholders.  

### 4. UI/UX Designer  
Designs the user interface and ensures a seamless user experience across all devices.  

### 5. Software Architect  
Designs the system architecture, deciding how frontend, backend, database, and APIs integrate.  

### 6. Developers  
- **Frontend Developers** → Build the user interface (React, HTML, CSS, JavaScript).  
- **Backend Developers** → Implement APIs, business logic, and handle server-side operations.  
- **Fullstack Developers** → Work across both frontend and backend.  

### 7. Quality Assurance (QA) Engineers  
Manually test features to ensure they meet requirements and are bug-free.  

### 8. Test Automation Engineers  
Write automated tests to reduce errors and improve release speed.  

### 9. DevOps Engineers  
Handle infrastructure, CI/CD pipelines, and deployment for scalability and reliability.  

## 🛠️ Technology Stack

This project leverages a modern technology stack to replicate the core features of Airbnb.  
Each technology plays a specific role in ensuring scalability, maintainability, and performance.  

- **Django**: A high-level Python web framework used to build the backend of the application, manage business logic, and serve RESTful APIs.  
- **PostgreSQL**: A powerful relational database system used for storing and managing user data, property listings, bookings, and transactions.  
- **GraphQL**: A query language that provides efficient data fetching by allowing clients to request only the data they need.  
- **HTML5 / CSS3**: For structuring and styling the front-end interface of the web application.  
- **JavaScript (ES6+)**: Adds interactivity and dynamic features to the client-side.  
- **Git & GitHub**: Version control and collaboration tools to track changes and manage project contributions.  
- **Docker (optional, if included)**: For containerization, ensuring consistency across different development and deployment environments.  

## 3. Database Design
**Objective:** Understand how the database will be structured.  

### Key Entities:
1. **Users**
   - Fields: `id`, `name`, `email`, `password_hash`, `role`
   - A user can own multiple properties and make multiple bookings.  

2. **Properties**
   - Fields: `id`, `owner_id`, `title`, `location`, `price`
   - Each property belongs to a user (owner).  

3. **Bookings**
   - Fields: `id`, `property_id`, `user_id`, `check_in`, `check_out`
   - A booking belongs to one property and one user.  

4. **Reviews**
   - Fields: `id`, `property_id`, `user_id`, `rating`, `comment`
   - A user can leave multiple reviews for different properties.  

5. **Payments**
   - Fields: `id`, `booking_id`, `amount`, `status`, `payment_date`
   - A payment is linked to a booking.  

### Relationships:
- A **User** can own many **Properties**.  
- A **Property** can have many **Bookings**.  
- A **Booking** belongs to both a **User** and a **Property**.  
- A **Review** belongs to a **User** and a **Property**.  
- A **Payment** is tied to a **Booking**.  