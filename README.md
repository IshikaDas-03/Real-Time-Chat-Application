# 💬 Real-Time Chat Application

This is a simple real-time group chat application built using **Spring Boot**, **WebSockets**, **STOMP (with SockJS)**, and **Bootstrap** for a responsive web UI. It allows multiple users to chat live in a single room, without needing to refresh the page.

---

## 📦 Technologies Used

| Layer         | Technology                     |
|--------------|---------------------------------|
| Backend      | Spring Boot, WebSocket (STOMP)  |
| Frontend     | HTML, JavaScript, Bootstrap 5   |
| Messaging    | STOMP over SockJS               |

---

## 🚀 Features

- 📡 Real-time messaging using WebSocket
- 🎨 Simple, responsive UI with Bootstrap 5
- 📥 Group chat support
- 🕓 Automatic scrolling on new messages
- 🔃 No page reloads needed
- 👨‍💻 Easily extendable (DB storage, authentication, emojis, etc.)

---

## 🧠 How It Works

1. Clients open a WebSocket connection to `/chat`.
2. Messages are sent from clients to the server at `/app/sendMessage`.
3. The server broadcasts the message to all clients subscribed to `/topic/messages`.

---
