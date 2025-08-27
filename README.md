# 💬 Chat App using MERN Stack (Final Year Project 2025)

A **real-time chat application** with an **Admin Dashboard** to monitor and manage everything happening in the app.  
Built with the **MERN stack** + **Socket.io** for instant communication.  
This README serves as both **documentation** and a **guide for setup, usage, and submission**.

---

## 📑 Table of Contents
1. [Abstract](#-abstract)
2. [Features](#-features)
3. [Tech Stack](#-tech-stack)
4. [Project Structure](#-project-structure)
5. [Installation](#-installation)
6. [Usage](#-usage)
7. [Database Schema](#-database-schema)
8. [Future Enhancements](#-future-enhancements)
9. [References](#-references)
10. [Author](#-author)

---

## 📌 Abstract
This project implements a **real-time chat application** with an integrated **Admin Dashboard** to monitor users, chats, and messages.  
It demonstrates modern web architecture using the **MERN stack (MongoDB, Express.js, React, Node.js)** and **Socket.io** for real-time communication.  

📊 **Use Case Diagram (Mermaid)**  


## ✨ Features

| Category           | Description                                                                  |
| ------------------ | ---------------------------------------------------------------------------- |
| 👥 User Features   | Real-time chat, group chat, typing indicators, message history, file sharing |
| 🔐 Auth System     | JWT authentication, secure login/signup, password hashing                    |
| 📊 Admin Dashboard | Monitor users, track active chats, manage system logs, block/unblock users   |
| ⚡ Performance      | Optimized WebSockets with Socket.io                                          |
| 🛠️ Developer      | Clean modular MERN stack codebase                                            |

---

## 🛠 Tech Stack

| Layer          | Technology                                 |
| -------------- | ------------------------------------------ |
| **Frontend**   | React (Vite), Tailwind CSS                 |
| **Backend**    | Node.js, Express.js                        |
| **Database**   | MongoDB, Mongoose                          |
| **Realtime**   | Socket.io                                  |
| **Auth**       | JWT, bcrypt                                |
| **Deployment** | Vercel (Frontend), Render/Heroku (Backend) |

---
````
chat-app-using-mern-stack-2025/
│
├── client/                  # Frontend (React + Vite)
│   ├── public/
│   ├── src/
│   ├── package.json
│   └── vite.config.js
│
├── server/                  # Backend (Node + Express)
│   ├── config/              # DB & environment configs
│   ├── controllers/         # Route logic
│   ├── models/              # Mongoose schemas
│   ├── routes/              # API endpoints
│   ├── server.js            # Entry point
│   └── package.json
│
├── README.md
├── LICENSE
└── .gitignore
````
---

## ⚙️ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/chat-app-using-mern-stack-2025.git
cd chat-app-using-mern-stack-2025
```

### 2️⃣ Setup Backend

```bash
cd server
npm install
```

Create `.env` file inside `/server`:

```env
PORT=5000
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_secret_key
```

Run backend:

```bash
npm run dev
```

### 3️⃣ Setup Frontend

```bash
cd ../client
npm install
npm run dev
```

* Frontend → `http://localhost:5173`
* Backend → `http://localhost:5000`

---

## ▶️ Usage

* Register or log in.
* Start one-to-one or group chats.
* Admin logs into dashboard to monitor activity.

**Example API Endpoints**:

| Method | Endpoint                | Description       |
| ------ | ----------------------- | ----------------- |
| POST   | `/api/auth/register`    | Register new user |
| POST   | `/api/auth/login`       | Authenticate user |
| POST   | `/api/chat/create`      | Create chat       |
| POST   | `/api/chat/message`     | Send message      |
| GET    | `/api/chat/admin/stats` | Admin analytics   |

---

## 🗄 Database Schema

| Collection   | Fields                                            |
| ------------ | ------------------------------------------------- |
| **Users**    | id, name, email, passwordHash, isAdmin, createdAt |
| **Chats**    | id, members\[], messages\[], createdAt            |
| **Messages** | id, chatId, senderId, content, timestamp          |

---

## 🚀 Future Enhancements

* Push notifications for new messages
* Video/voice calls via WebRTC
* End-to-End Encryption (E2EE)
* AI-powered chatbot integration
* Role-based access for admin/moderators

---

## 📚 References

* [React](https://reactjs.org)
* [Vite](https://vitejs.dev)
* [Node.js](https://nodejs.org)
* [Socket.io](https://socket.io)
* [MongoDB](https://www.mongodb.com)

---

## 👨‍💻 Author

**Chaman Ali Rana**
MERN Stack Developer | Final Year Project 2025 | AI Enthusiast

---

```
