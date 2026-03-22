# 📊 Analytics Slash Assistant (Colab MVP)

A notebook-based analytics assistant that enables non-technical users to generate business insights from raw CSV data using simple slash commands — powered by Python for computation and Claude for intelligent interpretation.

---

## 🚨 Problem

Most business users (PMs, analysts, operators) struggle to answer data questions because:

- They don’t know Python, SQL, or pandas  
- Data analysis requires multiple manual steps (cleaning → EDA → KPIs → insights)  
- Tools like notebooks are powerful but not accessible  
- Insights are often trapped behind technical workflows  

👉 Result: **slow decision-making and dependency on technical teams**

---

## 💡 Solution

This project introduces a **slash-command based analytics assistant** inside a Jupyter/Colab notebook.

Users can:

- Upload a CSV  
- Type simple commands like `/eda`, `/kpi`, `/summary`  
- Automatically generate insights without writing code  

The system combines:

- **Python** → deterministic analytics (truth layer)  
- **Claude (LLM)** → reasoning, summaries, and recommendations (intelligence layer)  

---

## ⚙️ How It Works

The notebook operates as a guided analytics pipeline:

1. User uploads a dataset  
2. User interacts via slash commands  
3. Python executes structured analysis  
4. Claude interprets outputs into business insights  
5. Results are stored in session state and reused across steps  

---

## 🧠 Architecture
User Input (/commands)
        ↓
Command Router (run_command)
        ↓
-------------------------------------
| Python Layer (Computation Engine) |
| - Data cleaning                   |
| - EDA                            |
| - KPI generation                 |
-------------------------------------
        ↓
-------------------------------------
| Claude Layer (Intelligence)      |
| - Goal interpretation            |
| - Executive summary              |
| - Report generation              |
-------------------------------------
        ↓
Final Output (Insights + Reports)
