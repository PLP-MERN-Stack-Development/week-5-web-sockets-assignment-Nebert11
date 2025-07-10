# NeChat App

A modern, full-featured real-time chat application built with React, Express, and Socket.io.

## 🚀 Overview
NeChat App is a real-time chat platform supporting global and private messaging, multiple chat rooms, file sharing, reactions, notifications, and more. It is designed for both desktop and mobile, with a focus on user experience and reliability.

---

## ✨ Features
- **Username-based authentication** (no registration required)
- **Global and multiple chat rooms**
- **Private messaging between users**
- **Real-time message delivery** with delivery acknowledgment
- **Typing indicators**
- **Online/offline user status**
- **Read receipts for private messages**
- **Message reactions (like, love, etc.)**
- **Emoji picker for messages**
- **File, image, and video sharing**
- **Unread message counts for rooms**
- **System messages for user join/leave**
- **In-app and browser notifications for new messages**
- **Sound notifications for new messages**
- **Message search within rooms**
- **Message pagination (infinite scroll)**
- **Reconnection logic for network issues**
- **Responsive design for desktop and mobile**
- **Persistent login (remembers user after reload)**

---

## 🛠️ Setup Instructions

### Prerequisites
- Node.js v18 or higher
- pnpm (or npm/yarn)

### Local Development
1. **Clone the repository:**
   ```sh
   git clone <your-repo-url>
   cd week-5-web-sockets-assignment-Nebert11
   ```
2. **Install server dependencies:**
   ```sh
   cd server
   pnpm install
   ```
3. **Install client dependencies:**
   ```sh
   cd ../client
   pnpm install
   ```
4. **Start the servers:**
   - In `server/`: `pnpm run dev`
   - In `client/`: `pnpm run dev`
5. **Open the app:**
   - Client: [http://localhost:5173](http://localhost:5173)
   - Server: [http://localhost:5000](http://localhost:5000)

### Environment Variables
- **Frontend (`client/.env`):**
  ```
  VITE_SOCKET_URL=http://localhost:5000
  ```
- **Backend (`server/.env`):**
  ```
  CLIENT_URL=http://localhost:5173
  ```
  *(Update these for production deployment!)*

---

## 🌐 Deployment

NeChat App can be deployed as a full-stack app on Render, Railway, or similar platforms.

### Steps:
1. **Build the React app:**
   ```sh
   cd client
   pnpm run build
   ```
2. **Copy the build output to the server:**
   - Copy contents of `client/dist` to `server/public`.
3. **Push to GitHub and deploy using your platform’s instructions.**
   - Set environment variables for production URLs.
   - Start command: `node server/server.js`

---

## 🧩 Project Structure
```
week-5-web-sockets-assignment-Nebert11/
├── client/         # React front-end
│   ├── src/
│   ├── public/
│   └── ...
├── server/         # Express/Socket.io back-end
│   ├── server.js
│   ├── public/     # Contains built React app for deployment
│   └── ...
└── README.md
```

---

## 📸 Live Link
*https://week-5-web-sockets-assignment-nebert11.onrender.com/*

---

## 📋 Assignment Tasks Checklist
- [x] Project setup (Express, Socket.io, React)
- [x] Core chat functionality (rooms, messages, typing, status)
- [x] Advanced features (private chat, file sharing, reactions, read receipts)
- [x] Real-time notifications (in-app, sound, browser)
- [x] Performance/UX (pagination, reconnection, search, responsive, persistent login)
- [x] Deployment

---


---

## 👤 Author
*NeChat App by [Nebert Ngari]* 