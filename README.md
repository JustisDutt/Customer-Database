**Live Demo:** https://customer-database-273912255588.us-west1.run.app 

# Customer Database Manager

## Overview
Customer Database Manager is a full-stack web application designed to manage client records securely and efficiently for small businesses. The system provides authenticated access to create, read, update, and delete customer data through a RESTful API and a simple web interface.

The project was built to demonstrate backend-first system design, secure authentication practices, and real-world cloud deployment using modern infrastructure tooling.

---

## Problem Statement
Many small businesses rely on spreadsheets or ad-hoc tools to track customer information, which leads to data inconsistency, poor access control, and limited scalability. This project addresses that gap by providing a centralized, authenticated system for managing customer records with a clean API and cloud-native deployment.

---

## System Architecture

**High-level flow:**
1. Client submits requests through a web interface or API.
2. Requests are authenticated and validated by the backend.
3. Business logic processes CRUD operations.
4. Data is persisted in a relational database.
5. Responses are returned via REST endpoints over HTTPS.

**Core components:**
- **Backend API:** Node.js and Express handling routing and business logic
- **Authentication:** Secure password hashing and credential validation
- **Database:** SQLite relational datastore
- **Deployment:** Containerized service running on Google Cloud Run

---

## Tech Stack

**Backend**
- Node.js
- Express
- REST APIs
- bcrypt authentication

**Database**
- SQLite
- SQL-based CRUD operations

**Frontend**
- HTML
- CSS
- JavaScript

**Cloud & DevOps**
- Google Cloud Run
- Cloud Build
- Artifact Registry
- Docker
- HTTPS with scale-to-zero deployment

---

## Scope and Constraints

**In Scope**
- User authentication
- Secure password storage
- Customer record CRUD operations
- Server-side validation
- Cloud-native deployment

**Out of Scope**
- Role-based access control
- Advanced analytics
- Horizontal database scaling
- Production-grade monitoring

These constraints are intentional to keep the system focused on core backend engineering fundamentals.

---

## Repository Structure

```
Customer-Database/
├── backend/
│   ├── routes/           # API route handlers
│   ├── middleware/       # Authentication and validation logic
│   ├── db/               # SQLite database logic
│   └── server.js         # Express app entry point
├── frontend/
│   ├── index.html
│   ├── styles.css
│   └── app.js
├── Dockerfile
├── cloudbuild.yaml
└── README.md
```

---

## Running the Project Locally

### Requirements
- Node.js 18+
- Docker (optional)

### Local Development
```bash
npm install
npm start
```

### Docker
```bash
docker build -t customer-database .
docker run -p 8080:8080 customer-database
```

---

## What This Project Demonstrates

- Designing secure RESTful APIs
- Implementing authentication correctly
- Structuring backend services for maintainability
- Deploying containerized applications to the cloud
- Bridging backend systems with a simple frontend

---

## Author
**Justis Dutt**  
- Portfolio: https://www.justisdutt.com  
- GitHub: https://github.com/JustisDutt  
- LinkedIn: https://www.linkedin.com/in/justis-dutt-951834224/

---
