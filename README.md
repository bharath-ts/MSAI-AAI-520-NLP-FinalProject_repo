# 🧠 Financial Agent: Multi-Agent AI Bot for Stock Recommendation

## 🚀 Project Overview
**Financial Agent (FA)** is a multi-agent financial intelligence system designed to autonomously collect market data, analyze stocks, evaluate risk, and recommend trades.  
It leverages a **modern Agentic AI architecture** that combines autonomous agents, dynamic workflow orchestration, and traditional business logic.

The system follows a hybrid design:
- 🤖 **45% Agent Functions:** 15 specialized AI agents for finance analytics  
- 🔄 **30% Workflow Patterns:** Dynamic orchestration, routing, and feedback learning  
- 💻 **25% Code Business Logic:** Rule-based computation, APIs, and I/O management  

---

## 🧩 Agentic Architecture Breakdown

### 🤖 Agent Functions (45%)
Fifteen autonomous agents collaborate to perform complex financial tasks via shared states and orchestrated communication.

| Agent Name | Responsibility |
|-------------|----------------|
| **MarketDataAgent** | Fetches live market feeds (Yahoo Finance / AlphaVantage) |
| **SentimentAgent** | Performs sentiment analysis on financial news and tweets |
| **FeatureEngineeringAgent** | Generates features from price history, volume, and indicators |
| **ModelTrainerAgent** | Trains ML models (RandomForest, XGBoost) for trend prediction |
| **PredictionAgent** | Generates buy/sell/hold predictions |
| **RiskAnalysisAgent** | Calculates VaR, Sharpe ratio, and exposure limits |
| **PortfolioAgent** | Allocates capital and optimizes portfolio diversification |
| **BacktestingAgent** | Validates strategies using historical data |
| **StrategyOptimizerAgent** | Tunes hyperparameters and trading thresholds |
| **PerformanceMonitorAgent** | Tracks ongoing model and agent performance |
| **ComplianceAgent** | Ensures trades follow regulatory and policy constraints |
| **LoggingAgent** | Handles structured logging and persistence |
| **NotificationAgent** | Sends alerts and updates to users |
| **EvaluationAgent** | Aggregates results and generates performance reports |
| **CoordinatorAgent** | Central orchestrator managing dependencies and workflow |

🧮 **Code Contribution:** ~45% — model intelligence, API integrations, and analytics.

---

### 🔄 Workflow Patterns (30%)
Implements a dynamic orchestration pipeline that routes data intelligently between agents.

Key patterns:
- **Task Delegation:** Coordinator assigns subtasks to relevant agents  
- **Parallel Execution:** Asynchronous data retrieval, analysis, and sentiment scoring  
- **Feedback Loop:** Continuous learning from market performance  
- **State Management:** Shared memory maintains context  
- **Error Recovery:** Fallback for failed API calls or incomplete streams  

🧮 **Code Contribution:** ~30% — orchestration logic, message passing, and monitoring.

---

### 💻 Code Business Logic (25%)
Handles deterministic processes outside of agent autonomy:
- Stock data pre-processing and transformation  
- Configuration management (API keys, environment)  
- Rule-based filtering for restricted sectors  
- Visualization and report export (Matplotlib, Pandas, JSON)

🧮 **Code Contribution:** ~25% — ensures control, consistency, and validation.

---

## ⚙️ Setup Instructions

### 1️⃣ Prerequisites
- Python **3.10+**
- Git
- Virtual environment (recommended: `venv` or `conda`)

### 2️⃣ Clone Repository
```bash
git clone https://github.com/yourusername/financial-agent.git
cd financial-agent
```

### 3️⃣ Create & Activate Virtual Environment
**For Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```
**For macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 4️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 5️⃣ Configure Environment Variables
Create a `.env` file in the root directory with your API keys:
```bash
ALPHAVANTAGE_API_KEY=your_api_key
YAHOO_FINANCE_API_KEY=your_api_key
```

### 6️⃣ Run Notebook or Script
Launch Jupyter Notebook:
```bash
jupyter notebook
```
Then open and run the main notebook: `Financial_Agent.ipynb`

Or run as a Python script (if available):
```bash
python main.py
```

### 7️⃣ (Optional) Export Reports
The system automatically saves logs, results, and charts in the `/output` directory.

---

## 🔁 Agentic Flow (Execution Pipeline)
1. CoordinatorAgent initializes workflow  
2. MarketDataAgent retrieves & cleans price data  
3. SentimentAgent collects & scores news  
4. FeatureEngineeringAgent prepares input vectors  
5. ModelTrainerAgent builds & validates ML models  
6. PredictionAgent generates trading signals  
7. RiskAnalysisAgent adjusts exposure thresholds  
8. PortfolioAgent optimizes asset allocation  
9. BacktestingAgent validates strategy  
10. EvaluationAgent compiles metrics  
11. NotificationAgent sends final insights  

---

## ⚙️ Tech Stack

| Layer | Technology |
|--------|-------------|
| **Language** | Python 3.10+ |
| **Data** | Pandas, NumPy, yfinance |
| **ML Models** | scikit-learn, XGBoost |
| **NLP** | spaCy, Transformers |
| **Visualization** | Matplotlib, Seaborn |
| **Agent Framework** | Custom lightweight orchestrator |

---

## 📈 Example Outputs
- 📊 Stock buy/sell recommendations  
- 🧮 Portfolio allocation summary  
- 💬 Sentiment polarity & trend score  
- ⚠️ Risk exposure analysis  
- 🧠 Model performance metrics (precision, recall, profit ratio)

---

## 📘 Notebook Guide

| Section | Description |
|----------|--------------|
| **1. Initialization** | Imports, configuration, environment setup |
| **2. Agent Definitions** | Specialized agent logic |
| **3. Workflow Orchestration** | Coordination and data routing |
| **4. Training & Prediction** | Model creation and inference |
| **5. Evaluation** | Metrics computation and visualization |
| **6. Output & Logging** | Export reports and logs |

---

## 🧭 Key Design Principles
- **Agent Autonomy:** Independent but context-aware modules  
- **Reusability:** Modular agents reusable across financial pipelines  
- **Transparency:** Logging and metrics for accountability  
- **Adaptability:** Real-time feedback updates models dynamically  

---

## 🧠 Architecture Summary

| Component | Description | Share |
|------------|--------------|-------|
| 🤖 Agent Functions | Specialized autonomous agents | 45% |
| 🔄 Workflow Patterns | Orchestration, routing, feedback loops | 30% |
| 💻 Code Business Logic | Deterministic data handling and visualization | 25% |

---

## 🧾 License
This project is released under the **MIT License**.  
You may freely use, modify, and distribute it with proper attribution.

---