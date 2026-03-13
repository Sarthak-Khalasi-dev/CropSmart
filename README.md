# 🌾 CropSmart — AI Crop Recommendation System

> Smart farming starts with smart data. CropSmart uses Machine Learning to recommend the best crops based on your soil, climate, and location.

---

## 📁 Project Structure

```
cropsmart/
├── frontend/          # React + Tailwind CSS (Vite)
├── backend/           # Node.js + Express + MongoDB
└── ml-model/          # Python Flask ML API
```

---

## ⚙️ Tech Stack

| Layer     | Technology                    |
|-----------|-------------------------------|
| Frontend  | React 18, Tailwind CSS, Vite  |
| Backend   | Node.js, Express.js           |
| Database  | MongoDB + Mongoose            |
| ML Model  | Python Flask                  |
| Auth      | JWT (jsonwebtoken)            |

---

## 🚀 Quick Setup

### 1. Clone & Install

```bash
# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install

# ML Model
cd ../ml-model
pip install -r requirements.txt
```

### 2. Environment Variables

Create `backend/.env`:
```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/cropsmart
JWT_SECRET=your_secret_key_here
CLIENT_URL=http://localhost:5173
ML_API=http://localhost:5001
```

### 3. Start All Services

**Terminal 1 — ML Model:**
```bash
cd ml-model
python app.py
# Running on http://localhost:5001
```

**Terminal 2 — Backend:**
```bash
cd backend
npm run dev
# Running on http://localhost:5000
```

**Terminal 3 — Frontend:**
```bash
cd frontend
npm run dev
# Running on http://localhost:5173
```

---

## ✅ All 15 Hackathon Features Implemented

| # | Feature | Where |
|---|---------|-------|
| 1 | Routing & Navigation | App.jsx + React Router |
| 2 | React Hooks | All pages (useState, useEffect, useRef, useContext) |
| 3 | State Management | AuthContext (Context API) |
| 4 | Authentication | JWT login/signup/protected routes |
| 5 | Theme Support | Dark/Light toggle in Navbar + Profile |
| 6 | Search, Filter, Sort | History.jsx + CropDatabase.jsx |
| 7 | Debouncing | useDebounce hook in search bars |
| 8 | Pagination | History + CropDatabase (backend + frontend) |
| 9 | CRUD Operations | Create/Read/Delete/Favorite recommendations |
| 10 | MongoDB Indexing | User (email), Recommendation (userId, location, soil) |
| 11 | MongoDB Aggregation | Stats page (crop count, soil stats, monthly usage) |
| 12 | API Integration | Axios + Express REST APIs + ML Flask API |
| 13 | Form Handling & Validation | Login, Signup, Dashboard, Profile |
| 14 | Responsive UI | Tailwind CSS — mobile + tablet + desktop |
| 15 | Error Handling | try-catch on all API calls, error messages |

---

## 📸 Pages

- `/` — Landing page
- `/signup` — Register
- `/login` — Sign in
- `/dashboard` — Crop recommendation form + results
- `/history` — Past recommendations (paginated, filterable)
- `/crops` — Crop database browser
- `/stats` — Analytics dashboard (MongoDB aggregation)
- `/profile` — Edit profile + theme toggle

---

## 🤖 ML Model API

**POST** `http://localhost:5001/predict`

```json
{
  "soilType": "black",
  "rainfall": 600,
  "temperature": 28,
  "location": "Gujarat"
}
```

**Response:**
```json
{
  "recommendations": [
    {
      "crop": "Cotton",
      "suitability": "Excellent",
      "expectedYield": "15-25 quintals/ha",
      "fertilizer": { "N": "120 kg/ha", "P": "60 kg/ha", "K": "60 kg/ha", "tip": "Use DAP at sowing" }
    }
  ]
}
```

---

© 2024 CropSmart — Built for Full Stack Hackathon
