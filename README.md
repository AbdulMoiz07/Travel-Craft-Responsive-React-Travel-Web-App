# 🌍 Travel Craft – Full Stack Travel App (React + MongoDB + OpenRouter)

A full-stack travel planning and exploration app built with **React** (frontend), **Express** (backend), and **MongoDB Atlas** (cloud database). Includes an **OpenRouter-powered chatbot**, hosted via Vercel CLI.

---

## 🚀 Project Setup Guide

### 🧩 1. Install All Dependencies

#### 📁 Frontend
```bash
cd src
npm install
```

#### 📁 Backend
```bash
cd backend
npm install
```

---

### 🔐 2. Setup Environment Variables (`.env` files)

#### 📁 A. Global `.env` (for OpenRouter API)
Create a `.env` file in the **root directory** (next to `src/` and `backend/`):

```env
OPENROUTER_API_KEY=your_openrouter_api_key_here
GEMINI_API_KEY=your gemini key
```

**Get your OpenRouter API key:**
1. Visit https://openrouter.ai
2. Sign up or log in
3. Go to Profile → API Keys → Generate a key
4. Paste it above

**Get your Gemini API key:**
🔑 Step 1: Get Your API Key from Google
Go to Google AI Studio

Log in with your Google account.

Click on your profile → API Keys

Click "Create API key"

Copy your key (starts with AIza...)
VITE_GEMINI_API_KEY=AIzaSyYourFullKeyHere
---

#### 📁 B. Backend `.env` (for MongoDB, Sessions, etc.)
Create another `.env` file inside the `backend/` folder:

```env
MONGO_URI=your_mongodb_uri_here
PORT=5000
SESSION_SECRET=your_session_secret_here
FRONTEND_URL=http://localhost:5173
NODE_ENV=development
```

**Get your MongoDB URI:**
1. Go to https://cloud.mongodb.com
2. Create a free MongoDB Atlas cluster
3. Click "Connect" → "Connect your application"
4. Copy the URI and replace `<username>`, `<password>`, and `<dbname>`

---

### 🧪 3. Run the Backend Server

```bash
cd backend
npm run check
```

✅ You should see: `MongoDB connected...`

---

### 🌐 4. Run the Frontend App

In a new terminal:

```bash
cd src
npm run dev
```

🔗 Your app will run at: `http://localhost:5173`

---

### 🤖 5. Run the Bot (OpenRouter via Vercel)

Open another terminal:

```bash
vercel dev
```

✅ Requirements:
- Vercel CLI installed → https://vercel.com/cli
- Run `vercel login` if needed
- Link the project by running `vercel` once

This will launch the chatbot locally using your OpenRouter API key.

---

## 🧾 Command Summary

| Task               | Command                     |
|--------------------|-----------------------------|
| Install frontend   | `cd src && npm install`     |
| Install backend    | `cd backend && npm install` |
| Run backend        | `cd backend && npm run check` |
| Run frontend       | `cd src && npm run dev`     |
| Run chatbot        | `vercel dev`                |

---

## 🛡️ Notes

- Do **not** commit `.env` files to GitHub.
- Local images are ignored using `.gitignore`.
- Environment variables securely handle API keys and database secrets.

---
If you're facing issue feel free to mail me at lcroft030@gmail.com
