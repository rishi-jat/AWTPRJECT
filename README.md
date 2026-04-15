# CollabBoard — Real-Time MERN Project Management System

## Overview
CollabBoard is a full-stack MERN application designed for collaborative project management using a Kanban-style board.  
It supports real-time updates, role-based access control, and secure authentication.

This project demonstrates practical usage of modern web development and DevOps concepts including containerization and production deployment.

---

## Live Demo
https://collabboard-realtime-nwpq.onrender.com  

Test Credentials:
- Email: admin@gmail.com  
- Password: Admin@123  

---

## Features

### Core Functionality
- Create and manage projects
- Kanban board with drag-and-drop cards
- Real-time synchronization across users
- Multi-user collaboration

### Authentication & Security
- JWT-based authentication
- Password hashing using bcrypt
- Protected API routes
- Role-Based Access Control (RBAC)

### Roles
- Admin → Full control (projects + boards + users)
- Manager → Manage boards and cards
- Developer → Work on assigned tasks

---

## Tech Stack

Frontend:
- React (Vite)
- React Router
- Axios
- @hello-pangea/dnd

Backend:
- Node.js
- Express.js

Database:
- MongoDB Atlas
- Mongoose

Real-time:
- Socket.io

DevOps:
- Docker
- Docker Compose
- Render deployment

---

## Project Structure

```
client/   → React frontend  
server/   → Express backend  
docker-compose.yml → local setup  
```

---

## How to Run

### Option 1: Docker
```
docker-compose up
```

### Option 2: Manual Setup

Backend:
```
cd server
npm install
npm run dev
```

Frontend:
```
cd client
npm install
npm run dev
```

---

## Environment Variables

Create `.env` inside `server/`:

```
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
CLIENT_URL=http://localhost:5173
```

---

## Key Concepts Used
- REST API design
- JWT authentication
- Role-based authorization (RBAC)
- Real-time communication with Socket.io
- MongoDB schema design

---

## Limitations
- No automated tests
- Basic UI (not fully optimized)
- No file upload support

---

## Future Improvements
- Add testing (unit + integration)
- Improve UI/UX
- Add notifications
- Add file attachments

---

## Author
Rishi Jat  
https://github.com/rishi-jat