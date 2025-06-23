# 🐾 Mokepon - Multiplayer Pokémon-Style Game

**Mokepon** is a Node.js-based multiplayer web application that allows users to join a game session, choose a Pokémon-style character, move on a map, and perform attacks. It's built using **Express** and utilizes **CORS** to enable client-server communication.

---

## 🚀 Technologies Used

- Node.js
- Express.js
- CORS
- HTML/CSS (client side)
- JavaScript (client and server side)

---

## 📦 Prerequisites

Make sure you have installed:

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [npm](https://www.npmjs.com/)

---

## 📂 Installation and Running the Server

```bash
git clone https://github.com/your-username/mokepon.git
cd mokepon
npm install
node index.js
```

This will start a local server on port 8080 by default.

---

## 📡 Server Endpoints

| Method | Route                             | Description                                        |
|--------|-----------------------------------|----------------------------------------------------|
| GET    | `/unirse`                         | Registers a new player and returns their ID        |
| POST   | `/mokepon/:jugadorId`             | Assigns a Mokepon to the player                    |
| POST   | `/mokepon/:jugadorId/posicion`    | Updates the player's position on the map           |
| POST   | `/mokepon/:jugadorId/ataques`     | Assigns selected attacks to the player             |
| GET    | `/mokepon/:jugadorId/ataques`     | Retrieves the player's attacks                     |

---

## 🧠 Game Logic (Server)

Each player is represented as an object with:
- A unique ID
- An assigned Mokepon
- Position (x, y)
- A list of attacks

The routes allow players to interact with each other through HTTP requests, simulating a real-time battle experience.

---

## 📁 Project Structure

```
Mokepon/
├── index.js              # Main server using Express
├── package.json          # Project dependencies and config
├── public/               # Client files (HTML, JS, CSS)
└── node_modules/         # Installed dependencies
```

---

## ⚖️ License

This project is licensed under the ISC license.
