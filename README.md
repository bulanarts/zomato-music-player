# 🎵 Zomato Music Player

A Spotify-inspired music player web app built as a learning project.

---

## 🤔 What is this project?

This is a full-stack music player app — meaning it has both a **frontend** (what you see) and a **backend** (what happens behind the scenes). Think of it like an iceberg — the frontend is the tip you see, the backend is everything underwater.

---

## 🛠️ Tech Stack (Tools Used)

Don't worry if these sound unfamiliar — here's what each one means in plain English!

### Frontend (What You See)

| Tool | What it does | Beginner analogy |
|------|-------------|-----------------|
| **React** | Builds all the UI pages and components (buttons, sidebar, player) | LEGO bricks — you build pieces and snap them together |
| **Vite** | Runs and builds the React app during development | The oven that bakes your LEGO pieces |
| **TypeScript** | The language used to write the frontend code (stricter version of JavaScript) | JavaScript with a spell-checker turned on |
| **TailwindCSS** | Handles all the styling — colors, layout, spacing | The paint and furniture for your house |
| **ShadCN UI** | Ready-made beautiful components so we don't build everything from scratch | IKEA furniture — pre-built, just assemble |
| **Zustand** | Manages the app's state — like currently playing song, volume, queue | The app's memory — remembers what's happening right now |

### Backend (What Happens Behind the Scenes)

| Tool | What it does | Beginner analogy |
|------|-------------|-----------------|
| **Node.js** | Runs the backend server | The kitchen of a restaurant |
| **Express** | Handles API routes — like `/get-songs`, `/login` | The waiter taking and delivering orders |
| **MongoDB** | Stores all data — songs, users, playlists | The fridge storing all ingredients |
| **Socket.io** | Handles real-time features like live listening together | An intercom between kitchen and front of house |
| **JavaScript** | The language used to write the backend code | Same language as the browser, just running on a server |

---

## 🔄 How They All Talk to Each Other

```
User clicks "Play Song"
        ↓
     React (UI updates)
        ↓
   Express API gets called
        ↓
  Node.js processes the request
        ↓
  MongoDB fetches the song data
        ↓
Socket.io sends updates to all listeners
        ↓
   React updates the UI in real time
```

---

## ✨ Features

- 🎵 Play music
- 📋 View playlists and queue
- 👤 User authentication (login / signup)
- 🔄 Real-time live listening with other users
- 💾 Persistent data stored in database

---

## 🚀 Getting Started

### Prerequisites (things you need installed first)
- [Node.js](https://nodejs.org) (v18 or higher)
- npm (comes with Node.js automatically)

### Installation

1. **Clone the project**
```bash
git clone https://github.com/yourusername/zomato-music-player.git
cd zomato-music-player
```

2. **Install frontend dependencies**
```bash
cd frontend
npm install
```

3. **Install backend dependencies**
```bash
cd backend
npm install
```

4. **Set up environment variables**

Create a `.env` file in the frontend folder:
```
VITE_CLERK_PUBLISHABLE_KEY=your_key_here
```

Create a `.env` file in the backend folder:
```
MONGODB_URI=your_mongodb_uri
PORT=3000
```

5. **Run the app**

Frontend:
```bash
npm run dev
```

Backend:
```bash
npm start
```

---

## 📁 Project Structure

```
zomato-music-player/
├── frontend/               # Everything the user sees
│   ├── src/
│   │   ├── components/     # Reusable UI pieces (buttons, cards)
│   │   ├── pages/          # Full pages (Home, Login, Player)
│   │   └── main.tsx        # App entry point
│   └── package.json
│
└── backend/                # Everything behind the scenes
    ├── routes/             # API endpoints (/songs, /users)
    ├── models/             # Database structure
    └── index.js            # Server entry point
```

---

## 👶 New to React or Vite?

Here are some helpful resources to get started:

- [What is React?](https://react.dev/learn) — Official React beginner guide
- [What is Vite?](https://vitejs.dev/guide/) — Vite getting started guide
- [What is Node.js?](https://nodejs.org/en/learn/getting-started/introduction-to-nodejs) — Node.js intro
- [What is MongoDB?](https://www.mongodb.com/basics) — MongoDB basics

---

## 📝 Notes

- This project was built as a learning exercise inspired by Spotify
- Frontend uses TypeScript, backend uses JavaScript — both are totally valid choices!
- Socket.io enables real-time features without needing to refresh the page

---

*Built with ❤️ as a learning project*
