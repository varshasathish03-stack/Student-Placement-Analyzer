# 🎓 Student Placement & Career Skill Intelligence System

An AI-driven platform for predicting student placement probabilities, identifying skill gaps, and providing personalized career guidance.

---

## 🌐 Quick Access URLs

| Service | Local URL | Description |
| :--- | :--- | :--- |
| **Frontend App** | **[http://localhost:5173](http://localhost:5173)** | Main Web Application UI (Vite + React) |
| **Backend API** | **[http://localhost:8000](http://localhost:8000)** | FastAPI Service Endpoint |
| **API Docs (Swagger)** | **[http://localhost:8000/docs](http://localhost:8000/docs)** | Interactive OpenAPI Documentation |
| **API Docs (ReDoc)** | **[http://localhost:8000/redoc](http://localhost:8000/redoc)** | ReDoc API Documentation |

---

## 📁 Shortcut Launch Files

For convenience, you can launch the application directly using shortcut files in the root directory:
- **`open_app.html`**: [`open_app.html`](file:///c:/Users/varsha/OneDrive/Documents/ML%20project/open_app.html) (Opens browser redirect)
- **`app_shortcut.url`**: [`app_shortcut.url`](file:///c:/Users/varsha/OneDrive/Documents/ML%20project/app_shortcut.url) (Windows Internet Shortcut)

---

## 🚀 Getting Started

### 1. Prerequisites
- Python 3.10+
- Node.js 18+ and `npm`

### 2. Run Backend Server
```bash
# Install Python dependencies
pip install -r requirements.txt

# Run FastAPI backend
python -m uvicorn backend.app.main:app --host 127.0.0.1 --port 8000 --reload
```

### 3. Run Frontend App
```bash
# Navigate to frontend
cd frontend

# Install Node dependencies
npm install

# Start Vite dev server
npm run dev
```

---

## 🏗️ Project Architecture

```
ML project/
├── backend/             # FastAPI backend services, routes, models & database
│   └── app/
│       ├── core/        # Security, JWT auth, and config
│       ├── database.py  # SQLite DB connection
│       ├── main.py      # Application entrypoint
│       ├── models.py    # SQLAlchemy database models
│       ├── routers/     # API endpoints (auth, prediction, skills)
│       └── services/    # Business logic & ML inference
├── frontend/            # Vite + React + TypeScript UI
│   ├── src/
│   │   ├── components/  # Navigation, cards, charts
│   │   ├── context/     # Auth state context provider
│   │   ├── pages/       # Login, Dashboard, Analytics, Predictor views
│   │   └── config.ts    # API base URL configuration
│   └── index.html
├── ml/                  # ML pipeline: data cleaning, EDA, model training
├── DEPLOYMENT_GUIDE.md  # Production deployment guide (Render + Vercel)
├── open_app.html        # Quick launch HTML redirect
└── app_shortcut.url     # Quick launch Windows shortcut
```

---

## 📑 Production Deployment

Refer to [`DEPLOYMENT_GUIDE.md`](file:///c:/Users/varsha/OneDrive/Documents/ML%20project/DEPLOYMENT_GUIDE.md) for full deployment instructions to cloud hosting services (Render & Vercel).
