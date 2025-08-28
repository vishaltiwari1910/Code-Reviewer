# Code Reviewer

A real-time AI-powered code review tool built with **React (Vite)** frontend and **Node.js/Express** backend. Paste your code and get instant review suggestions using Google Generative AI.

---

## 🛠 Features

- Real-time syntax highlighted code editor
- AI-powered code review
- Markdown formatted review output
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

yaml
Copy code

---

## ⚡ Installation & Setup

### 1️⃣ Backend

1. Navigate to backend folder:
```bash
cd backend
Install dependencies:

bash
Copy code
npm install
Create a .env file in the backend folder:

env
Copy code
GOOGLE_GEMINI_KEY=YOUR_GOOGLE_API_KEY
PORT=5000
Start backend server (local development):

bash
Copy code
node server.js
Backend API endpoint:

bash
Copy code
POST http://localhost:5000/ai/get-review
2️⃣ Frontend
Navigate to frontend folder:

bash
Copy code
cd Frontend
Install dependencies:

bash
Copy code
npm install
Create .env file in frontend folder:

env
Copy code
VITE_API_BASE_URL=http://localhost:5000/ai
Start development server:

bash
Copy code
npm run dev
Open in browser: http://localhost:5173

To create production build:

bash
Copy code
npm run build
🌐 Deployment
Backend (Render)
Connect GitHub repo to Render

Set environment variables:

Copy code
GOOGLE_GEMINI_KEY, PORT
Deploy Node.js service

Frontend (Vercel)
Connect GitHub repo to Vercel

Set environment variable:

ini
Copy code
VITE_API_BASE_URL=https://your-backend-url.onrender.com/ai
Deploy React + Vite project

🧩 Usage
Open the frontend app in browser

Paste code into editor

Click Review

Get AI-powered review in Markdown format

🔐 Security
.env files are excluded via .gitignore

Never commit API keys to GitHub

⚙️ Tech Stack
Frontend: React, Vite, PrismJS, react-simple-code-editor, Axios, Markdown rendering

Backend: Node.js, Express, CORS, Google Generative AI

Deployment: Vercel (Frontend), Render (Backend)
