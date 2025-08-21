# Credit Card Clients – Good vs Bad Payer Classification

## 📌 Project Overview
This project analyzes a **credit card clients dataset** to classify customers into:
- **Good Payers**: Regularly pay ≥70% of their outstanding balance
- **Bad Payers**: Pay less than 70% of their balance

The goal is to build a **predictive model** that can help financial institutions estimate whether a **new customer** is likely to be a good or bad payer.

---

## 🗂 Dataset
- Source: `CC GENERAL.csv`
- Customers: 8,950
- Features: Balance, Credit Limit, Purchases, Payments, Cash Advance, etc.
- Target: `good_payer` (binary, engineered)

---

## 🔎 Methodology
1. **Data Cleaning**
   - Removed duplicates
   - Handled missing values
   - Scaled numeric features
2. **Feature Engineering**
   - Payment ratio = `PAYMENTS / BALANCE`
   - Good/Bad Payer definition
3. **Exploratory Data Analysis (EDA)**
   - Distribution plots, boxplots, correlation heatmap
   - Segment analysis for good vs bad payers
4. **Modeling**
   - Logistic Regression (baseline)
   - Random Forest (advanced)
5. **Evaluation**
   - Accuracy, Precision, Recall, F1, ROC-AUC
   - Confusion Matrix
   - ROC and Precision-Recall Curves
6. **Business Insights**
   - Good payers have higher payments and more responsible usage patterns
   - Segment profiles by balance & risk
7. **Deployment**
   - Best model saved (`joblib`)
   - Inference function for new customers

---

## 📊 Results
- **Good Payer Share:** ~84%  
- **Best Model:** Random Forest  
- **ROC-AUC:** ~0.90 (Cross-Validation)  
- **Feature Importance:** Balance, Payments, Credit Limit are most predictive  

---

## 🛠 Tech Stack
- Python (pandas, numpy, scikit-learn, matplotlib, seaborn)
- Jupyter Notebook
- Joblib (model persistence)

---

## 🚀 How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/credit-card-good-payer.git
   cd credit-card-good-payer
   ```
2. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:
   ```bash
   jupyter notebook cctv.ipynb
   ```

---

## 📈 Example Dashboard
In addition to the ML notebook, an interactive Power BI dashboard shows:
- Good vs Bad Payer distribution
- Balance quantiles
- Risk categories
- Payments vs Minimum Payments comparison

---

## 📌 Author
Prepared as part of a **machine learning project on credit risk analysis**.  
