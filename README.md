# 🛡️ QualityGuardian AI
### AI Smart Manufacturing Quality Agent

> **Continuous Quality Intelligence for Smart Factories** — Detecting defects, predicting failures, and recommending corrective actions in real-time.

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104+-green.svg)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/React-18+-61DAFB.svg)](https://reactjs.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 📖 Overview

**QualityGuardian AI** is an intelligent manufacturing quality monitoring agent that combines three AI paradigms to deliver **zero-defect manufacturing**:

- 🔍 **Computer Vision** — Real-time surface defect detection (scratches, dents, cracks)
- 📈 **Time-Series Forecasting** — Predicts upcoming quality degradation from sensor streams
- 📊 **Statistical Process Control (SPC)** — Monitors process stability with X-bar/R charts, Cp/Cpk
- 🤖 **Gemini AI Reasoning** — Generates human-readable corrective actions & root cause analysis

The system acts as a **24/7 autonomous quality inspector** — turning raw camera feeds and sensor data into actionable quality intelligence.

---

## ✨ Key Features

### 🔍 Computer Vision Module
- Real-time defect detection using lightweight CNN (MobileNetV2-based)
- Supports scratches, dents, cracks, and surface anomalies
- Confidence scoring + bounding box overlay
- Image upload & live camera feed support

### 📈 Time-Series Forecasting
- ARIMA / LSTM-based quality prediction
- Multi-sensor correlation (temperature, pressure, vibration)
- Forecast next N products' quality risk
- Anomaly detection on sensor streams

### 📊 Statistical Process Control (SPC)
- X-bar & R control charts
- UCL / LCL / CL auto-calculation
- Cp / Cpk process capability indices
- Western Electric rule violation detection

### 🤖 Gemini AI Agent
- Root-cause analysis of defects
- Human-readable corrective action recommendations
- Context-aware reasoning across all 3 modules
- Priority-based action suggestions

### 🎨 Interactive Dashboard
- Real-time KPIs (FPY, defect rate, OEE)
- Live sensor graphs (WebSocket)
- Defect gallery with filters
- Alert management (UCL breach, defect spike)
- Exportable reports (PDF/CSV)

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| **Backend** | Python 3.10+, FastAPI, Uvicorn |
| **Database** | SQLite + SQLAlchemy ORM |
| **Computer Vision** | OpenCV, TensorFlow/Keras (MobileNetV2) |
| **Time-Series** | statsmodels (ARIMA), scikit-learn |
| **SPC** | NumPy, Pandas (custom engine) |
| **AI Reasoning** | Google Gemini API (`google-generativeai`) |
| **Real-time** | WebSockets (FastAPI) |
| **Frontend** | React 18, Vite, TailwindCSS |
| **Charts** | Recharts / Chart.js |
| **State** | Zustand / Redux Toolkit |
| **HTTP Client** | Axios |
| **Auth** | JWT (python-jose) |
| **Icons** | Lucide React |

---

## 🏗️ Architecture



---

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.10+
- Node.js 18+
- Git
- Google Gemini API Key ([Get here](https://aistudio.google.com/app/apikey))

### 1️⃣ Clone Repository

```bash
git clone https://github.com/vishakha2121/AI-Powered-Real-Time-Manufacturing-Quality-Intelligence.git
cd AI-Powered-Real-Time-Manufacturing-Quality-Intelligence

# Create virtual environment
python -m venv venv

# Activate (Windows)
venv\Scripts\activate

# Activate (Mac/Linux)
source venv/bin/activate

# Install dependencies
cd backend
pip install -r requirements.txt


cd frontend
npm install
npm run dev