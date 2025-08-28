# Code Reviewer

A real-time AI-powered code review tool built with **React (Vite)** frontend and **Node.js/Express** backend. Paste your code and get instant review suggestions using Google Generative AI.

---

## 🛠 Features

- Real-time syntax-highlighted code editor
- AI-powered code review
- Markdown-formatted review output
- Frontend deployed on **Vercel**, backend on **Render**
- Supports multiple programming languages

---

## 📂 Project Structure

Code-Reviewer/
├── Frontend/ # React + Vite frontend
│ ├── src/
│ ├── public/
│ └── package.json
├── backend/ # Node.js + Express backend
│ ├── src/
│ │ ├── controllers/
│ │ ├── routes/
│ │ └── services/
│ ├── server.js
│ └── package.json
├── .gitignore
└── README.md



---

## ⚡ Installation & Setup

### 1️⃣ Backend

1. Navigate to backend folder:
```bash
cd backend
npm install

GOOGLE_GEMINI_KEY=YOUR_GOOGLE_API_KEY
PORT=5000
node server.js

POST http://localhost:5000/ai/get-review


cd Frontend
npm install


VITE_API_BASE_URL=http://localhost:5000/ai


npm run dev

GOOGLE_GEMINI_KEY, PORT


https://code-reviewer-7dmy.onrender.com/ai


VITE_API_BASE_URL=https://your-backend-url.onrender.com/ai

https://code-reviewer-rose.vercel.app/




Usage

Open the frontend app in browser

Paste your code into the editor

Click Review

Get an AI-powered code review in Markdown format

🔐 Security

.env files are excluded via .gitignore

Never commit API keys to GitHub

⚙️ Tech Stack

Frontend: React, Vite, PrismJS, react-simple-code-editor, Axios, Markdown rendering

Backend: Node.js, Express, CORS, Google Generative AI

Deployment: Vercel (Frontend), Render (Backend)


Notes

Make sure backend server is running before frontend tries to fetch reviews.

For production, update VITE_API_BASE_URL to point to deployed backend URL.

Large code snippets may take a few seconds for AI review.
