# Logeasy-AI
# 🧠 **LogEasy — AI-Powered Fintech Log Intelligence Platform**

> **“LogEasy — An AI-powered fintech reliability assistant that predicts, analyzes, and automates log analysis in real-time.”**

---

## 📘 **Overview**

**LogEasy** is an intelligent log management and analytics system designed for **Fintech reliability and compliance**.  
It connects to servers or APIs, fetches logs automatically, and uses **AI + predictive analytics** to detect, explain, and prevent system issues — all through a clean, real-time dashboard.

---

## 🚀 **Core Features**

| Feature | Description | Benefit |
|----------|--------------|----------|
| 🧾 **Fetch logs directly from servers/APIs** | Automatically pull logs from APIs, servers, or uploaded files | Saves time & reduces manual errors |
| 🔍 **Smart log search & filtering** | Filter logs by keyword, date, service, or severity | Speeds up debugging |
| 📊 **Analytics & visualizations** | Charts showing error frequency, uptime, and service health | Quick insights for dev teams |
| 🤖 **AI-generated insights** | Detect recurring issues and suggest root causes | Smarter decision-making |
| 📈 **Predictive alerts** | Forecast potential failures before they occur | Prevents downtime |
| 📄 **Report generation (PDF/DOCX)** | Automated audit-ready reports | For compliance and documentation |
| 🕒 **Real-time dashboard** | Live status of system health & error counts | One unified monitoring view |
| 🧮 **Compliance-ready storage** | Store logs formatted for **RBI audit compliance** | Reduces manual compliance effort |

---

## 🏗️ **System Architecture**

```
Frontend (React.js) → Backend API (FastAPI) → AI Engine (scikit-learn/NLP)
                           ↓
                   Database (PostgreSQL/SQLite)
                           ↓
                      Reports & Analytics
```

- **Frontend**: React.js dashboard for real-time monitoring & visualization  
- **Backend**: FastAPI REST API managing logs, insights, and report generation  
- **AI Engine**: Python ML modules for log classification, anomaly detection & predictions  
- **Database**: PostgreSQL or SQLite for log & report persistence  
- **Reports**: Automated generation of PDF/DOCX summaries  

---

## 🧩 **Tech Stack**

| Layer | Technology |
|--------|-------------|
| **Frontend** | React.js, Axios, Chart.js, TailwindCSS |
| **Backend** | FastAPI, Uvicorn, Pydantic |
| **AI/ML** | scikit-learn, pandas, NLTK/spaCy |
| **Database** | PostgreSQL / SQLite |
| **Visualization** | Plotly.js / Chart.js |
| **Reporting** | ReportLab, python-docx |
| **Containerization** | Docker, Docker Compose |

---

## ⚙️ **Project Structure**

```
LogEasy/
├── backend/              # FastAPI backend
│   ├── app/
│   │   ├── api/          # API routes
│   │   ├── core/         # Config & utils
│   │   ├── services/     # Log parsing, report generation
│   │   ├── ml_engine/    # AI models & predictors
│   │   ├── database/     # ORM models & DB connection
│   │   ├── tests/        # Automated tests
│   │   └── main.py       # FastAPI entry point
│   ├── requirements.txt
│   └── Dockerfile
│
├── frontend/             # React.js dashboard
│   ├── src/
│   │   ├── components/   # Dashboard components
│   │   ├── pages/        # Main views
│   │   ├── services/     # Axios & WebSocket logic
│   │   ├── utils/        # Formatters, helpers
│   │   ├── styles/       # Tailwind/CSS files
│   │   ├── App.jsx
│   │   └── index.js
│   ├── package.json
│   └── README.md
│
├── data/                 # Sample logs & reports
├── models/               # Trained ML models + notebooks
├── scripts/              # Utility scripts (train, simulate, generate reports)
├── docker-compose.yml
└── README.md
```

---

## 🧰 **Installation & Setup**

### 🪄 **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/logeasy.git
cd logeasy
```

### 🧱 **2. Backend Setup (FastAPI)**
```bash
cd backend
python -m venv venv
source venv/bin/activate   # (on Windows: venv\Scripts\activate)
pip install -r requirements.txt
```

Run the backend:
```bash
uvicorn app.main:app --reload
```
Backend will start at 👉 `http://localhost:8000`

---

### 💻 **3. Frontend Setup (React)**
```bash
cd frontend
npm install
npm start
```
Frontend will start at 👉 `http://localhost:3000`

---

### 🐳 **4. (Optional) Run with Docker Compose**
```bash
docker-compose up --build
```
This will launch **FastAPI + React + PostgreSQL** together.

---

## 🧠 **AI Components**

| Module | Function |
|--------|-----------|
| `classifier.py` | Categorizes logs (Error, Warning, Info) using NLP |
| `anomaly_detector.py` | Detects unusual spikes in errors |
| `predictor.py` | Forecasts potential failures based on trends |
| `pdf_report.py` | Generates summary reports for teams or audits |

🧪 Models are stored in:  
`/models/trained/log_classifier.pkl`, `/models/trained/anomaly_model.pkl`

---

## 📊 **Dashboard Features**

- **Search & Filter Logs**: by keyword, service, or time  
- **Visual Analytics**: dynamic graphs showing trends  
- **AI Insights Panel**: natural-language summaries  
- **Real-Time Monitoring**: system health overview  
- **Export Reports**: PDF/DOCX audit summaries  

---

## 🧾 **API Endpoints (FastAPI)**

| Method | Endpoint | Description |
|--------|-----------|--------------|
| `POST` | `/upload` | Upload or fetch logs |
| `GET`  | `/logs` | Get parsed and filtered logs |
| `GET`  | `/insights` | Retrieve AI-generated insights |
| `POST` | `/predict` | Predict future failures |
| `GET`  | `/report/download` | Download audit/report file |

Swagger UI available at:  
👉 `http://localhost:8000/docs`

---

## 🔐 **Environment Variables (`.env`)**

| Variable | Description |
|-----------|--------------|
| `DATABASE_URL` | PostgreSQL / SQLite connection string |
| `API_KEY` | Optional auth for fetching logs |
| `MODEL_PATH` | Path to saved ML models |
| `LOG_STORAGE_PATH` | Directory for raw logs |

Example file: `.env.example`

---

## 🧭 **Roadmap**

- [ ] Add authentication (JWT)  
- [ ] Integrate real-time WebSocket updates  
- [ ] Deploy models via FastAPI background tasks  
- [ ] Add alerting system (Slack/Email notifications)  
- [ ] Build RBI compliance module (auto-format logs)  
- [ ] Deploy on AWS EC2 or Render  

---

## 🧑‍💻 **Contributing**

Contributions are welcome!  
Please open a PR or issue if you’d like to help improve LogEasy.  

**Guidelines:**
- Follow PEP8 for Python
- Use semantic commits
- Add docstrings and comments
- Test new features before pushing

---

## 🧮 **License**

This project is licensed under the **MIT License** — free to use and modify with attribution.

---

## 💬 **Contact**

👨‍💻 **Project Lead:** Your Name  
📧 Email: your.email@example.com  
🌐 GitHub: [github.com/yourusername](https://github.com/yourusername)

---

## 🏁 **Final Tagline**

> 💡 *“LogEasy — Making fintech reliability smarter, faster, and audit-ready.”*
