# 🛒 Australian Grocery Retail Price Analysis

## 📌 Project Overview

This project analyzes grocery product pricing data collected from **coles.com.au** across Australia. The main goal is to investigate whether promotional pricing labeled as **“Special”** truly offers value to consumers when prices are normalized by unit size.

The analysis focuses on **unit price fairness**, **category-level pricing behavior**, and **estimated consumer overpayment** caused by misleading promotions.

---

## 🎯 Key Business Questions

1. Are *Special* products genuinely cheaper than non-special products?
2. Which product categories misuse the *Special* label the most?
3. How volatile are prices within the same category?
4. How much money do consumers potentially lose due to misleading promotions?

---

## 📂 Dataset Description

* **Source:** Coles Australia (Grocery Department)
* **Coverage:** Multiple Australian states and cities
* **Rows:** ~488,000 products
* **Key Fields:**

  * Category / Sub-category
  * Package price
  * Unit price
  * Package size (text-based: e.g. `500g`, `1kg`)
  * Special flag (`is_special`)
  * Location (state, city, postal code)

> ⚠️ Raw CSV files exceed GitHub size limits and are therefore excluded. A data dictionary and processing logic are fully documented in the notebook.

---

## 🧹 Data Cleaning & Preparation

* Parsed package size from text into numeric grams/ml
* Normalized prices to **price per 100g/ml** for fair comparison
* Handled missing values and inconsistent unit formats
* Verified calculated unit prices against provided values

---

## 🔍 Analysis Summary

### 1️⃣ Special vs Non-Special Pricing

* Special products have lower *average package prices*
* **Median unit prices show little to no real discount**
* Many specials are cheaper per package but **not cheaper per unit**

### 2️⃣ Category Abuse of “Special” Labels

* Certain categories consistently label products as *Special* despite higher-than-median unit prices
* Indicates promotional pricing is not always consumer-friendly

### 3️⃣ Price Dispersion & Outliers

* Significant price variation exists within the same categories
* High dispersion increases the risk of consumer overpayment
* Outliers identified using IQR-based detection

### 4️⃣ Estimated Consumer Loss 💰

* Calculated excess cost where *Special* unit prices exceed category baselines
* Aggregated losses reveal categories with the highest potential consumer harm

---

## 📊 Key Insights

* Promotional pricing does **not guarantee better value**
* Unit price normalization is critical for fair comparison
* Some categories systematically misuse discount labels
* Consumers may overpay significantly due to misleading promotions

---

## 🛠️ Tools & Technologies

* Python (Pandas, NumPy)
* Jupyter Notebook
* Matplotlib / Seaborn
* Statistical testing (Mann–Whitney U)
* Git & GitHub

---

## 📁 Project Structure

```
retail-sales-analytics/
├── data/                # Dataset schema & notes (CSV excluded)
├── notebooks/           # Data analysis notebooks
│   └── retail_analysis.ipynb
├── sql/                 # SQL queries (optional extension)
├── dashboard/           # BI dashboards (Power BI / Tableau)
└── README.md
```

---

## 🚀 Future Improvements

* Time-based price trend analysis
* Brand-level pricing fairness
* Predictive model for misleading promotions
* Interactive dashboard deployment

---

## 👤 Author

**Arman Rostami**
Aspiring Data Analyst / Data Engineer
Australia 🇦🇺

---

## 📌 Disclaimer

This project is for educational and analytical purposes only. Pricing insights do not represent official claims against retailers.
