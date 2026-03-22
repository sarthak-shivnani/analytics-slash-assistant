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
<img width="367" height="394" alt="image" src="https://github.com/user-attachments/assets/0111869f-6bec-48ef-a45e-6ba6872e5201" />


👉 Key principle:

- **Python computes facts**  
- **Claude explains meaning**

---

## 💻 Supported Slash Commands

| Command | Description |
|--------|------------|
| `/help` | Show available commands |
| `/goal <text>` | Define business objective + generate analysis brief (Claude) |
| `/status` | Show current workflow progress |
| `/profile` | Dataset structure + schema summary |
| `/data-quality` | Missing values, duplicates, outliers |
| `/clean` | Conservative data cleaning |
| `/eda` | Exploratory data analysis |
| `/kpi` | KPI summary for numeric columns |
| `/root-cause <issue>` | Diagnostic leads for investigation |
| `/visualize` | Basic charts |
| `/summary` | Executive summary (Claude) |
| `/report` | Final business report (Claude) |

---

---

## 🛠 Tech Stack

- Python (pandas, numpy, seaborn, matplotlib)  
- Google Colab / Jupyter Notebook  
- Anthropic Claude API (LLM layer)  
- Markdown + notebook interface  

---

## ⚠️ Limitations

This is an MVP and has the following constraints:

- Works only with structured CSV datasets  
- Limited handling of very large datasets  
- No domain-specific KPI logic (generic analysis)  
- Root-cause analysis is heuristic (not causal inference)  
- Visualizations are basic  
- Requires manual upload (no live data connections)  
- Claude outputs depend on prompt quality  

---

## 🚀 Roadmap (Future Improvements)

- Smarter visualization selection  
- Advanced root-cause analysis (segmentation, comparisons)  
- Custom analysis command (`/custom-analysis`)  
- Multi-dataset support (joins)  
- Streamlit-based UI (move beyond notebook)  
- Domain-specific analytics (SaaS, finance, marketing)  
- Guardrails for statistical validity  
- Automated insight ranking (impact + novelty)  

---

## 🎯 Why This Project Matters

This project demonstrates:

- Building **end-to-end analytics systems**  
- Combining **deterministic computation + LLM reasoning**  
- Designing **user-friendly data interfaces**  
- Translating raw data → actionable business insights  

👉 This is the direction of modern analytics tools.

---

## 📌 How to Run

1. Open the notebook in Google Colab  
2. Run all setup cells  
3. Upload your CSV file  
4. Use slash commands via the input cell  

---

## 📣 Author

**Sarthak Shivnani**  
MS Business Analytics — UT Austin  

---

## ⭐ Final Note

This is not just a notebook.  
It is a step toward **AI-assisted analytics systems for non-technical users**.
