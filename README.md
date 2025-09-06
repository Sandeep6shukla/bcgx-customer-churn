# BCG X Virtual Internship — Customer Churn Prediction

This repository contains my work from the **BCG X Data Science Virtual Internship** project, focused on predicting customer churn and identifying the role of **price sensitivity** in churn behavior.

---

## 📂 Repository Structure
├── data/
│ ├── client_data.csv
│ ├── price_data.csv
│ ├── clean_data_after_eda.csv
│ ├── clean_data_with_features.csv
│ └── model_metrics.json
│
├── notebooks/
│ ├── EDA_BCGX_Task2.ipynb
│ ├── feature_engineering_extended_with_summary.ipynb
│ └── modelling_rf.ipynb
│
├── reports/
│ ├── client_summary_slide.pdf
│ ├── Executive_Summary_Filled.pptx
│ └── Executive_Summary_Visual.pptx
│
├── README.md
└── .gitignore


---

## 🧾 Project Overview
- **Objective:** Validate whether price sensitivity is the main driver of churn and build a predictive model.  
- **Datasets Used:**
  - **Client data**: customer tenure, consumption, margins, etc.
  - **Pricing data**: variable & fixed prices over time.
  - **Churn indicator**: whether the customer churned or not.

---

## 🔍 Methodology
1. **Exploratory Data Analysis (EDA)**  
   - Inspected data types, distributions, and missing values.  
   - Identified price change patterns across customers.  

2. **Feature Engineering**  
   - Created tenure, consumption ratios, margin differences.  
   - Added price-based features: averages, volatility, spreads.  
   - Built interaction features (e.g., `estimated_annual_bill`).  

3. **Modeling with Random Forest**  
   - 75/25 train-test split, stratified.  
   - Achieved ~85% accuracy and strong recall on churn prediction.  
   - Top features: price changes, annual bill estimates, tenure.  

---

## 📈 Key Findings
- **Price sensitivity is a major churn driver** — off-peak price increases correlate strongly with churn.  
- **Tenure and consumption ratios** also affect churn likelihood.  
- The **Random Forest model** provides actionable predictions to identify high-risk customers.  

---

## 💡 Business Impact
- Enables **early identification of churn-prone customers**.  
- Supports **targeted retention strategies** (loyalty programs, tailored pricing).  
- Protects recurring revenue — even a **5% reduction in churn** can safeguard significant margins.  

---

## 🚀 Next Steps
- Validate with larger datasets.  
- Pilot targeted offers for high-risk customers.  
- Collaborate with marketing to implement churn-reduction strategies.  

---

## ⚙️ How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/Sandeep6shukla/bcgx-customer-churn.git
   cd bcgx-customer-churn



