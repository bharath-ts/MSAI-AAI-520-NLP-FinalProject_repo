# 🧠 Financial Agent: Multi-Agent AI Bot for Stock Recommendation

## 🚀 Project Overview
**Financial Agent (FA)** is a multi-agent financial intelligence system designed to autonomously collect market data, analyze stocks, and generate investment research reports.  
It leverages a **modern Agentic AI architecture** built on LangGraph that combines autonomous agents, dynamic workflow orchestration, and structured data retrieval.

The system follows a hybrid design:
- 🤖 **Agent Functions:** 4 specialized AI agents for research orchestration  
- 🔄 **Workflow Patterns:** Dynamic routing, conditional execution, and evaluator-optimizer loops  
- 💻 **Code Business Logic:** Tool wrappers, data processing, and report generation  

---

## 🧩 Agentic Architecture Breakdown

### 🤖 Agent Functions 
Four autonomous agents collaborate to perform comprehensive financial research via shared states and orchestrated communication.

| Agent Name | Responsibility |
|-------------|----------------|
| **ProfilerAgent** | Fetches company profile (sector, industry, business summary) |
| **PlannerAgent** | Generates dynamic research plans based on company characteristics |
| **ToolWorkers** | Execute data retrieval (news, financials, SEC filings, market data) |
| **EvaluatorAgent** | Quality assurance with iterative refinement loop |

🧮 **Code Contribution:** — agent intelligence, LLM reasoning, and adaptive planning.

---

### 🔄 Workflow Patterns 
Implements a dynamic LangGraph orchestration pipeline with conditional routing and feedback loops.

Key patterns:
- **Dynamic Planning:** Planner adapts research sequence based on company sector/industry  
- **Conditional Routing:** Research router determines next step based on plan state  
- **Tool Orchestration:** Sequential execution of data retrieval tools  
- **Evaluator-Optimizer Loop:** Iterative report refinement with quality gates  
- **State Management:** Shared ResearchState maintains context across agents  

🧮 **Code Contribution:** — LangGraph workflow, conditional edges, and state management.

---

### 💻 Code Business Logic 
Handles deterministic processes and tool integrations:
- **Tool Wrappers:** NewsAPI, yfinance, SEC API integrations  
- **Data Processing:** Article preprocessing, sentiment classification, entity extraction  
- **Report Generation:** Structured investment analysis with SWOT framework  
- **Error Handling:** Graceful fallbacks for API failures  

🧮 **Code Contribution:** — ensures reliability, data quality, and structured outputs.

---

## ⚙️ Setup Instructions

### 1️⃣ Prerequisites
- Python **3.10+**
- Git
- Virtual environment (recommended: `venv` or `conda`)

### 2️⃣ Clone Repository
```bash
git clone https://github.com/bharath-ts/MSAI-AAI-520-NLP-FinalProject_repo.git
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
pip install langchain langgraph langchain-google-genai newsapi-python yfinance sec-api pandas numpy
```

### 5️⃣ Configure API Keys
Set up your API keys in the notebook or as environment variables:
```python
# In notebook cells
Gemini_API_key = 'your_gemini_api_key'
news_api = 'your_newsapi_key'
sec_api = 'your_sec_api_key'
```

**Required APIs:**
- **Google Gemini API:** For LLM reasoning and text generation
- **NewsAPI:** For financial news retrieval
- **SEC API:** For regulatory filings access

### 6️⃣ Run the Notebook
Launch Jupyter Notebook:
```bash
jupyter notebook
```
Then open and run: `Financial_Agent_Multi_Agent_AI_Bot_for_Stock_recommendation.ipynb`

### 7️⃣ Test the System
Run test cases with different stock symbols:
```python
# Test with different companies
app.invoke({'stock_symbol': 'AAPL'})  # Tech company
app.invoke({'stock_symbol': 'DUK'})   # Utility company  
app.invoke({'stock_symbol': 'NVDA'})  # AI/semiconductor company
```

---

## 🔁 Agentic Flow (Execution Pipeline)
1. **ProfilerAgent** → Fetches company profile and initializes state
2. **PlannerAgent** → Generates dynamic research plan based on company characteristics
3. **Research Router** → Determines next step from plan
4. **Tool Workers** → Execute data retrieval in planned sequence:
   - `fetch_news` → News chaining with sentiment analysis and entity extraction
   - `fetch_financials` → Key financial metrics from yfinance
   - `fetch_sec_filings` → Risk factors and MD&A from SEC filings
   - `fetch_market_data` → Market performance and analyst recommendations
5. **Report Generator** → Creates comprehensive investment analysis
6. **Evaluator Agent** → Quality assurance with iterative refinement
7. **Final Report** → Outputs polished investment recommendation

---

## ⚙️ Tech Stack

| Layer | Technology | Purpose |
|--------|-------------|---------|
| **Language** | Python 3.10+ | Core implementation |
| **Agent Framework** | LangGraph | Workflow orchestration and state management |
| **LLM Integration** | LangChain + Google GenAI | Agent reasoning and text generation |
| **Data Sources** | yfinance, NewsAPI, SEC API | Market data, news, and regulatory filings |
| **Data Processing** | Pandas, NumPy | Data manipulation and analysis |
| **Output Parsing** | JSON, String parsers | Structured data extraction |

---

## 📈 Example Outputs
- 📊 **Company Profile:** Sector, industry, business summary
- 📰 **News Analysis:** Sentiment classification, entity extraction, trend insights
- 💰 **Financial Metrics:** Revenue, net income, assets, liabilities
- ⚖️ **SEC Insights:** Risk factors and management discussion summaries
- 📈 **Market Context:** Market cap, 52-week range, beta, analyst consensus
- 📋 **Investment Report:** Comprehensive SWOT analysis with buy/sell/hold recommendation

---

## 📘 Notebook Structure

| Section | Description |
|----------|--------------|
| **1. Introduction** | Project overview and motivation |
| **2. Libraries & Environment** | Dependencies and API setup |
| **3. Data Sources & Tools** | Tool definitions and integrations |
| **4. Agent Functions** | Profiler, Planner, Tool Workers, Evaluator |
| **5. Workflow Patterns** | LangGraph implementation with conditional routing |
| **6. Evaluation** | Quality assurance and refinement loops |
| **7. Results & Insights** | End-to-end testing and analysis |
| **8. Limitations & Future Work** | Current constraints and improvement areas |
| **9. How to Run** | Reproducibility instructions |
| **10. Conclusion** | Summary and key achievements |

---

## 🧭 Key Design Principles
- **Adaptive Planning:** Research sequence adapts to company characteristics
- **Grounded Retrieval:** All analysis backed by real market data
- **Iterative Refinement:** Quality gates ensure report quality
- **Modular Architecture:** Reusable agents and tools
- **Transparency:** Full logging and state tracking

---

## 🧠 Architecture Summary

| Component | Description | 
|------------|--------------|
| 🤖 Agent Functions | Profiler, Planner, Tool Workers, Evaluator 
| 🔄 Workflow Patterns | LangGraph orchestration, conditional routing, feedback loops 
| 💻 Code Business Logic | Tool wrappers, data processing, report generation 

---

## 🧾 License
This project is released under the **MIT License**.  
You may freely use, modify, and distribute it with proper attribution.

---

## 👥 Team
**Not-A-Bot (Group -7)**
- Jasmeet Kaur
- Himanshu Kumar  
- Bharath TS

**Course:** AAI-520 — Final Project
