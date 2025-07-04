# 💬 Real-Time Chat App

A full-stack real-time chat application built using **React.js**, **Node.js**, **Express.js**, **MongoDB**, and **Socket.io**. This app allows users to register, log in, and exchange messages in real time. Built with a modular and scalable architecture using contexts, custom hooks, and web sockets.

---

## 📁 Project Structure

The project is divided into **three main parts**:

1. **Client** – Frontend React application
2. **Server** – Backend REST API using Node.js and Express
3. **Socket** – Real-time connection using Socket.IO

---

## 🚀 Features

- User registration and login
- One-to-one real-time chat
- Chat list with recent messages
- Online/offline user status tracking
- Notifications for unread messages
- Custom React hooks for efficient data fetching
- Responsive and clean UI using React-Bootstrap
- Local storage authentication
- Modular code using Context API

---

## 🔧 Folder Breakdown

### 1. `client/` (Frontend)
The client handles the user interface and interaction logic.

#### 📦 Folders:
- **assets/** – Static files like logos and icons.
- **components/** – Reusable UI components such as:
  - `Navbar`, `UserChats`, `PotentialChats`, `ChatBox`, `Notifications`
- **context/** – Global state using:
  - `AuthContext` for authentication
  - `ChatContext` for managing chat and socket state
- **hooks/** – Custom hooks:
  - `useFetchRecipient` – fetch recipient details
  - `useFetchLatestMessage` – get latest message in a chat
- **pages/** – Main pages:
  - `Register`, `Login`, `Chat`
- **utils/** – Utility files:
  - `services.js` – for GET/POST requests
  - `unreadNotifications.js` – filters unread messages

### 2. `server/` (Backend)
Handles business logic and connects to MongoDB.

#### 🧠 Modules:
- **controllers/** – Business logic for:
  - `userController.js`, `chatController.js`, `messageController.js`
- **routes/** – API routes:
  - `user.js`, `chat.js`, `message.js`
- **models/** – MongoDB models:
  - `User`, `Chat`, `Message`
- **database/** – MongoDB connection using Mongoose

### 3. `socket/` (Socket Server)
Establishes and manages real-time socket connections between users using **Socket.io**.

---

## 🛠 Tech Stack

- **Frontend**: React, React Bootstrap, Context API
- **Backend**: Node.js, Express.js, MongoDB, Mongoose
- **Real-Time**: Socket.io
- **Security**: JWT (JSON Web Tokens), bcrypt for password hashing

---

## 🧪 How to Run the App Locally

### 🔁 Clone the Repository

```bash
git clone https://github.com/Ankit-Singh1234/chatApp.git
cd chatApp
