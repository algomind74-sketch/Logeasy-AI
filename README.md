# ⚡ LogEasy – AI-Powered Log Analysis & Monitoring Tool  

### 🧠 Developed by Team Innovators:  
**Chanchal | Tushar | Sourav Yadav | Rajnikant**

---

## 🌍 Overview  

**LogEasy** is an **AI-driven platform** designed to automate log analysis and monitoring for large-scale software systems — especially in **FinTech** environments.  
It drastically reduces the time developers spend analyzing logs, from **25–30 minutes to under 2 minutes**, by combining all key functions — fetching, filtering, analyzing, and reporting — into one smart dashboard.  

> 💡 Think of LogEasy as a one-stop AI tool replacing Kibana, Grafana, and manual debugging.

---

## 🚨 Problem Statement  

FinTech systems like UPI, payment gateways, and banking apps generate **millions of logs every day**.  
Developers currently have to:
- Switch between multiple tools (Kibana, Grafana, Splunk).  
- Manually search, filter, and interpret logs.  
- Spend excessive time diagnosing root causes.  

This causes:
- ⚠️ Delays in resolving production issues  
- 💸 Poor system uptime & customer experience  
- 🧾 Compliance challenges with RBI audits  

---

## 💡 Our Solution – LogEasy  

**LogEasy integrates all log-related operations into a single, intelligent platform** powered by AI.  
Here’s what it offers:

| 🚀 Feature | 💬 Description |
|-------------|----------------|
| 🧾 **Fetch Logs** | Automatically retrieves logs from servers or APIs. |
| 🔍 **Smart Search & Filter** | Instantly search logs by date, service, or keywords. |
| 📊 **Visual Analytics** | Interactive graphs & metrics of system health and errors. |
| 🤖 **AI Insights** | Detects recurring issues & provides summarized insights. |
| 🔮 **Predictive Analysis** | Anticipates system failures based on log history. |
| ⚡ **Real-Time Dashboard** | Live status view of errors, uptime, and critical services. |
| 📈 **Compliance Reports** | Generates RBI-ready reports automatically. |

---

## 🧩 Tech Stack  

### **Backend**
- 🧩 **FastAPI (Python)** – REST API for AI integration  
- 🤖 **Scikit-learn / TensorFlow** – ML & predictive analysis  
- 🗄️ **PostgreSQL / SQLite** – Log & metadata storage  
- 📊 **Plotly / Matplotlib** – For data visualization  

### **Frontend**
- ⚛️ **React.js** – Dynamic, real-time dashboard  
- 🎨 **Tailwind CSS** – Sleek UI design  
- 🔌 **Axios + WebSocket** – API & live updates  

### **DevOps / Tools**
- 🐳 Docker – Containerization  
- 🧰 GitHub – Version control  
- 🧪 Postman – API testing  

---

## 🧠 AI Model Architecture  

The ML engine in LogEasy performs **3 core tasks**:

1. **Log Classification** → Categorizes logs as Error / Warning / Info.  
2. **Anomaly Detection** → Flags unusual spikes or abnormal activity.  
3. **Predictive Modeling** → Predicts potential service failures.  

### 🧾 ML File Descriptions  
| File | Purpose |
|------|----------|
| `preprocess.py` | Cleans and prepares raw logs |
| `classifier.py` | Classifies log types using NLP |
| `anomaly_detector.py` | Detects system anomalies |
| `predictor.py` | Predicts possible future failures |
| `train_models.py` | Trains and stores AI models |

---

## 📂 Folder Structure  
