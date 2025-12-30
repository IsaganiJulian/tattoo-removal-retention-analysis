# InkImpact: Strategic Retention & LTV Intelligence 💉

### ✈️ Project Overview
**InkImpact** is a data science solution developed for **The UnTattoo Parlor** to solve two critical business problems: high financial leakage through client churn and inefficient marketing spend. By analyzing thousands of session logs, I identified specific milestones where the business was losing nearly 44% of its revenue and redirected marketing efforts toward high-Lifetime Value (LTV) channels.

---
### 📂 Repository Structure
This project follows a modular data science structure to ensure reproducibility and scalability as the analysis moves from EDA to Predictive Modeling.

```text
├── data/
│   ├── processed/          # Cleaned data and feature-engineered sets
|   |── raw/                # Original, unaltered CSV logs  
│   └── models/             # Future: Saved ML models (.pkl)
├── notebooks/              # Research & Development
│   ├── 01_retention_eda.ipynb    # Phase 1: Diagnostic Leakage Analysis
│   └── 02_churn_prediction.ipynb # Phase 2: Predictive Modeling (In Progress)
|   └── 03_churn_prediction.ipynb # Phase 3: Survival Analysis (In Progress)
├── reports/                # Stakeholder Deliverables
│   ├── figures/            # Visual assets for Portfolio/Hugo
│   └── final_report_v1.pdf # Consolidated business findings
├── src/                    # The "Engine" (Modular Python Scripts)
│   ├── loader.py           # Reusable data cleaning pipeline
│   ├── features.py         # Engineering session velocity & pain proxies
│   └── viz_theme.py        # Standardized visualization styles
|   └── README.md           # Project documentation
├── requirements.txt        # Environment dependencies
---

### 💼 The Business Challenge
* **The Leakage Problem:** The Parlor lacked visibility into *when* clients were dropping off, leading to thousands in unrealized revenue.
* **The Acquisition Problem:** Marketing resources were being spent on high-volume but low-value channels like Facebook Ads.

---

### ⚙️ Technical Architecture
I built a diagnostic pipeline in Python to transform raw session data into actionable marketing strategy.

#### **Task 1: Retention Funnel Analysis**
* **Milestone Mapping:** Calculated retention rates across 10+ session intervals.
* **Findings:** Identified a **43.8% drop-off between Session 1 and 2**, and a secondary "fatigue" point at Session 6.

#### **Task 2: LTV & Channel Optimization**
* **LTV Modeling:** Aggregated revenue by acquisition source to find the "True ROI" of each channel.
* **Correlation Intelligence:** Discovered a **0.90 correlation** between session consistency (`Days_Since_Prior`) and total value, proving that long-term commitment is the primary driver of profitability.

---

### 🔍 Key Business Insights
* **Top Performing Channel:** **Tattoo Artist Referrals** produce clients with the highest retention and LTV.
* **Underperforming Channel:** **Facebook Ads** and **Word of Mouth** leads have the lowest LTV, suggesting a need for better lead qualification.
* **The "First-Visit" Crisis:** Almost half of all marketing spend is wasted if a client does not book their second appointment.

---

### 🚀 Strategic Recommendations
1. **Automated Intervention:** Launch an SMS "Second Session" incentive for Google/Instagram leads within 48 hours of their first appointment.
2. **Budget Reallocation:** Shift 20% of Facebook Ad budget into a **Tattoo Artist Referral Partnership** program.
3. **Bundled Pricing:** Create "Commitment Packages" for 5+ sessions to capitalize on the high correlation between session volume and LTV.

---

### 🛠️ Tech Stack
**Python** (Pandas, Seaborn, Matplotlib, NumPy) | **Jupyter** | **Git**