# DataIQ — AI-Powered Real-Time Data Intelligence Platform

![DataIQ Banner](https://img.shields.io/badge/DataIQ-AI%20Powered-00d4ff?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react)
![Kafka](https://img.shields.io/badge/Apache%20Kafka-Streaming-black?style=for-the-badge&logo=apachekafka)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688?style=for-the-badge&logo=fastapi)
![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker)

> Transforming raw data into real intelligence — built for Next-Level Product Sprint 2026

---

## 🚀 What Is DataIQ?

DataIQ is a production-grade AI-powered real-time data intelligence platform that allows anyone — regardless of technical background — to upload data, ask questions in plain English, and get instant AI-powered insights.

No SQL knowledge required. No data science degree needed. Just ask your data anything.

---

## 🎯 Problem Statement

Every business today generates massive amounts of data — but 90% of it goes completely unused because:

- ❌ Analyzing data requires expensive data scientists
- ❌ Writing SQL queries requires technical knowledge
- ❌ Real-time monitoring requires complex infrastructure
- ❌ Generating reports takes days of manual work
- ❌ Predictions require dedicated ML engineers

---

## ✅ How DataIQ Solves It

| Problem | DataIQ Solution |
|---------|----------------|
| Complex SQL queries | Plain English AI queries powered by Groq LLaMA 3 |
| No real-time monitoring | 3 live Kafka streams with automatic anomaly detection |
| Expensive predictions | Built-in AI forecasting with confidence scores |
| Manual report generation | One-click professional PDF report generation |
| Static dashboards | Connect any REST API for live data ingestion |

---

## ✨ Features

- 📁 **CSV Upload** — Upload any CSV, XLSX, or JSON file and instantly analyze it
- 🌐 **Live API Connection** — Connect any REST API for real-time data streaming
- 💬 **AI Chat** — Ask questions in plain English, get instant AI answers
- 📡 **Kafka Streaming** — 3 simultaneous real-time data streams with anomaly detection
- 🔮 **Predictions** — AI-powered forecasting for 7, 30, and 90 day horizons
- 📄 **PDF Reports** — One-click professional report generation
- ⚠️ **Anomaly Detection** — Automatic detection of unusual patterns in data
- 🔍 **AI Insights** — Automatic insight generation from your data

---

## 🏗️ Architecture

DATA SOURCES
├── CSV / XLSX / JSON Upload
├── REST API Connection (any URL)
└── Apache Kafka Streams (3 live streams)
↓
INGESTION & PROCESSING LAYER
├── Kafka Producer / Consumer
├── Pandas Data Processing
└── Data Cleaning & Schema Detection
↓
STORAGE LAYER
├── PostgreSQL (primary data store)
└── Redis (caching)
↓
AI / LLM INTELLIGENCE LAYER
├── Groq LLaMA 3 70B (natural language)
├── NL to SQL Conversion
├── Insight Generation
├── Anomaly Detection
└── Predictive Analytics (Linear Regression)
↓
PRESENTATION LAYER
├── React.js Dashboard
├── Real-Time Charts
├── AI Chat Interface
├── Kafka Stream Monitor
└── PDF Report Generator


---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Frontend** | React.js, Vite, Custom CSS |
| **Backend** | Python, FastAPI, Uvicorn |
| **AI / LLM** | Groq API, LLaMA 3 70B |
| **Streaming** | Apache Kafka, Zookeeper |
| **Database** | PostgreSQL |
| **Cache** | Redis |
| **Data Processing** | Pandas, NumPy |
| **HTTP Client** | Axios, HTTPX |
| **Reports** | ReportLab |
| **Infrastructure** | Docker, Docker Compose |

---

## 📁 Project Structure
hack-project/
├── backend/
│ ├── main.py
│ ├── requirements.txt
│ ├── api/
│ │ ├── upload.py
│ │ ├── query.py
│ │ ├── stream.py
│ │ └── reports.py
│ ├── pipeline/
│ │ ├── kafka_producer.py
│ │ └── kafka_consumer.py
│ ├── database/
│ │ └── postgres.py
│ ├── ai/
│ │ ├── llm_client.py
│ │ ├── nl_to_sql.py
│ │ ├── insight_generator.py
│ │ └── predictor.py
│ └── reports/
│ └── pdf_generator.py
│
└── frontend/
└── dataiq-final/
├── package.json
├── vite.config.js
└── src/
├── App.jsx
├── components/
│ ├── LandingPage.jsx
│ ├── Navbar.jsx
│ ├── DashboardPage.jsx
│ ├── PredictionsPage.jsx
│ └── ReportPage.jsx
├── services/
│ └── api.js
└── styles/
└── global.css


---

## ⚙️ Setup & Installation

### Prerequisites

Make sure you have these installed:
- Docker Desktop
- Python 3.11+
- Node.js 18+
- Git

### Step 1 — Clone The Repository

```bash
git clone https://github.com/YOURUSERNAME/dataiq.git
cd dataiq
```

### Step 2 — Set Up Environment Variables

```bash
cp .env.example .env
```

Open `.env` and add your keys:


Get your free Groq API key at: **console.groq.com**

### Step 3 — Start Docker Infrastructure

```bash
docker-compose up -d
```

Verify containers are running:
```bash
docker ps
```

You should see 4 containers:
- ✅ Kafka
- ✅ Zookeeper
- ✅ PostgreSQL
- ✅ Redis

### Step 4 — Start Backend

```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --reload
```

Backend runs at: **http://localhost:8000**

API Documentation: **http://localhost:8000/docs**

### Step 5 — Start Frontend

Open a new terminal tab:

```bash
cd frontend/dataiq-final
npm install
npm run dev
```

Frontend runs at: **http://localhost:5173**

---

## 🧪 Testing The Platform

### 1. Upload CSV Data
- Go to **http://localhost:5173**
- Click **CSV Upload** tab
- Upload any CSV file
- Ask questions in the chat

### 2. Connect Live API
- Click **Live API** tab
- Paste this URL:
