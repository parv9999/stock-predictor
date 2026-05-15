# 📈 AI-Powered Stock & Crypto Prediction System

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org/)
[![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![TextBlob](https://img.shields.io/badge/TextBlob-NLP-8A2BE2?style=for-the-badge)](https://textblob.readthedocs.io/)
[![CoinMarketCap](https://img.shields.io/badge/CoinMarketCap-API-1452F5?style=for-the-badge&logo=coinmarketcap&logoColor=white)](https://coinmarketcap.com/api/)
[![ngrok](https://img.shields.io/badge/ngrok-Public%20Hosting-1F1E37?style=for-the-badge&logo=ngrok&logoColor=white)](https://ngrok.com/)

> A machine learning–based financial analytics platform that fetches real-time crypto & stock data, runs predictive ML models, scores market sentiment via NLP, and delivers intelligent **BUY / SELL / HOLD** signals through a live Flask dashboard.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Core Features](#core-features)
- [System Architecture](#system-architecture)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Key Functionalities](#key-functionalities)
- [Resume Highlights](#resume-ready-highlights)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

---

## 📖 Overview

The **AI-Powered Stock & Crypto Prediction System** simulates an intelligent financial forecasting environment by combining:

- 🔴 **Live market data** via CoinMarketCap API
- 🤖 **Multiple ML algorithms** for price forecasting
- 🧠 **NLP sentiment analysis** to gauge market mood
- 🚦 **Signal generation** — BUY, SELL, or HOLD
- 📊 **Real-time visualization** of prices and predictions
- 🌍 **Public Flask dashboard** via ngrok tunneling

---

## 🚀 Core Features

### 📊 Real-Time Market Data Fetching
- CoinMarketCap API integration for live crypto prices
- Fetches current prices, historical trends & market movement data
- Fully automated data retrieval pipeline

### 🤖 AI/ML Prediction Engine
Implements multiple ML algorithms for financial forecasting:

| Algorithm | Purpose |
|---|---|
| Linear Regression | Baseline price trend forecasting |
| Time-Series Models | Short-term price movement prediction |
| Trend Forecasting | Pattern recognition & direction analysis |
| Multi-library Experimentation | Comparative model accuracy testing |

### 🧠 Sentiment Analysis Engine
- **TextBlob**-based NLP scoring on market text inputs
- Outputs: Positive score, Negative score, Neutral interpretation
- Feeds directly into trading signal accuracy

### 📈 Data Visualization
- Real-time price graph generation
- Trend & movement visualization
- Prediction vs. actual comparison charts
- Built using Python plotting libraries (Matplotlib)

### 🌍 Flask Web Deployment
- Browser-accessible prediction dashboard
- Live prediction interface & real-time interaction
- **ngrok** tunneling for instant public URL access

---

## 🏗️ System Architecture

```
CoinMarketCap API
        ↓
  Data Collection & Preprocessing
        ↓
  ┌──────────────────────────────┐
  │     Sentiment Analysis       │
  │     (TextBlob NLP Engine)    │
  └──────────────┬───────────────┘
                 │
  ┌──────────────▼───────────────┐
  │  ML Prediction Models        │
  │  Linear Regression           │
  │  Time-Series Forecasting     │
  │  Trend Pattern Recognition   │
  └──────────────┬───────────────┘
                 │
      Signal Generation
      BUY │ SELL │ HOLD
                 │
      Flask Backend Deployment
                 │
      ngrok → Public Dashboard
```

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| **Language** | Python |
| **Backend** | Flask |
| **ML & Data Science** | scikit-learn, Pandas, NumPy |
| **NLP & Sentiment** | TextBlob |
| **Visualization** | Matplotlib |
| **Market Data** | CoinMarketCap API |
| **Public Hosting** | ngrok |
| **Dev Tools** | Git, GitHub, VS Code |

---

## 📁 Project Structure

```
stock-predictor/
│
├── fetch_data.py              # CoinMarketCap API — live data fetching
├── sentiment_score.py         # TextBlob NLP sentiment scoring
├── predict_models.py          # ML prediction algorithms
├── prediction_5min.py         # Short-term (5-min) price forecasting
├── signal_prediction.py       # BUY / SELL / HOLD signal generation
├── plot_price_graph.py        # Real-time price & trend visualization
├── flask_deployment.py        # Flask backend server
├── public_url.py              # ngrok public tunnel setup
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Getting Started

### Prerequisites
- Python 3.8+
- CoinMarketCap API Key (free tier) → [Get here](https://coinmarketcap.com/api/)
- ngrok account → [ngrok.com](https://ngrok.com/)

### 1. Clone the Repository

```bash
git clone https://github.com/parv9999/stock-predictor.git
cd stock-predictor
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

If `requirements.txt` is missing:

```bash
pip install flask pandas numpy matplotlib scikit-learn textblob requests
```

### 3. Configure API Key

In `fetch_data.py`, set your CoinMarketCap key:

```python
API_KEY = "your_coinmarketcap_api_key_here"
```

### 4. Run the Application

```bash
python flask_deployment.py
```

Or test individual modules:

```bash
python fetch_data.py          # Verify live data fetch
python sentiment_score.py     # Test sentiment scoring
python predict_models.py      # Run prediction models
python signal_prediction.py   # Test signal generation
```

### 5. Access the Dashboard

- **Local:** `http://127.0.0.1:5000`
- **Public:** ngrok URL printed in terminal on startup

---

## 💡 Key Functionalities

### ✅ Real-Time Price Monitoring
- Live crypto price fetching with dynamic market updates
- Continuous trend tracking pipeline

### ✅ Predictive Analytics
- Future price forecasting using trained ML models
- Short-term movement & historical pattern analysis

### ✅ Intelligent Signal Generation
Signals are produced by combining:
- Market trend direction (from ML models)
- Sentiment polarity (from TextBlob NLP)
- Predicted movement probability

Output: **🟢 BUY** | **🔴 SELL** | **🟡 HOLD**

### ✅ Sentiment-Driven Analysis
NLP sentiment scores simulate market psychology — combining textual market mood with numerical prediction models for more informed signal accuracy.

---

## 💼 Resume-Ready Highlights

> Copy-paste ready for your CV or LinkedIn:

- Developed an AI-powered financial prediction platform integrating real-time market APIs, NLP sentiment analysis, and multiple ML forecasting models
- Implemented intelligent BUY/SELL/HOLD signal generation combining ML predictions with TextBlob sentiment scores
- Built a Flask-based web dashboard with ngrok public access for live prediction interaction and testing
- Designed end-to-end data visualization pipelines for real-time price monitoring and trend comparison

---

## 🔮 Future Enhancements

- [ ] LSTM & Transformer deep learning models
- [ ] Real-time auto trading bot integration
- [ ] Portfolio management dashboard
- [ ] Advanced technical indicators (RSI, MACD, Bollinger Bands)
- [ ] Live news sentiment tracking pipeline
- [ ] Multi-crypto & stock ticker support
- [ ] Cloud deployment on AWS
- [ ] User authentication system
- [ ] Automated trading execution engine

---

## 👤 Author

**Parv Chauhan**
B.Tech Computer Science — VIT Bhopal University

- GitHub: [@parv9999](https://github.com/parv9999)
- Email: [parvchauhan36@gmail.com](mailto:parvchauhan36@gmail.com)

---

<p align="center">🧠 Where Machine Learning meets Market Intelligence.</p>
