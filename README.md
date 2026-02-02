# 🎨 Collaborative Canvas – Real-Time Drawing App

Collaborative Canvas is a real-time drawing application where multiple users can draw together on the same canvas.

It uses HTML5 Canvas, Vanilla JavaScript, Node.js, and Socket.IO to provide fast and smooth real-time collaboration.

---

## 📁 Project Structure

collaborative-canvas/
│
├── client/                 # Frontend (Canvas UI)
│   ├── index.html
│   ├── style.css
│   ├── canvas.js
│   ├── websocket.js
│   └── main.js
│
├── server/                 # Backend (Socket.IO Server)
│   ├── server.js
│   ├── drawing-state.js
│   ├── rooms.js
│   └── package.json
│
├── node_modules/
├── .gitignore
├── ARCHITECTURE.md
├── package-lock.json
└── README.md


---

## 🚀 Features

- Real-time drawing with multiple users
- Live cursor movement of other users
- Brush and eraser tools
- Color picker and brush size option
- Undo and redo for each user
- Clear only your own drawings
- Multiple room support
- Very low latency using WebSockets

---

## 🛠️ Tech Stack

### Frontend
- HTML5 Canvas
- Vanilla JavaScript
- Socket.IO Client
- CSS

### Backend
- Node.js
- Express.js
- Socket.IO Server

---

## ⚙️ Local Development Setup

### 1️⃣ Clone the repository

git clone https://github.com/yourusername/repo-name.git
cd collaborative-canvas

---

### 2️⃣ Backend Setup

cd server
npm install
npm start

Backend runs at:
http://localhost:3000

---

### 3️⃣ Frontend Setup

Open client/index.html using:
- VS Code Live Server  
OR  
- Any static server

---

## 🌐 Deployment (Render)

### Backend (Web Service)
- Root Directory: server
- Build Command: npm install
- Start Command: npm start

### Frontend (Static Site)
- Root Directory: client
- Publish Directory: client
- Build Command: (leave empty)

---

## 🔗 Connect Frontend to Backend

In client/websocket.js:

Replace:
const socket = io();

With:
const socket = io("https://YOUR_BACKEND.onrender.com");

---

## 🧪 Testing

Open the app in multiple browser tabs.
Draw in one tab and see changes instantly in others.

---

## 🤝 Contributing

Pull requests are welcome.
Feel free to improve features or fix bugs.
