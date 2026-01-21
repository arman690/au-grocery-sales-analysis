# AU Grocery Sales Analytics

**End-to-end analysis of Australian grocery products from Coles, including pricing, stock, and category insights. Cleaned, analyzed, and visualized for business analytics and dashboard projects.**

---

## Dataset
This project uses a grocery products dataset extracted from the Grocery department of [coles.com.au](https://www.coles.com.au/).  
It includes information on a selected list of categories of grocery products in Australia, including pricing and stock details.

**Columns include:**
- `Postal Code`: The postal code of the store or product location.
- `Category` / `Subcategory`: Product classification.
- `Product Group` / `Product Name` / `Brand` / `SKU Number`
- `Package Price` / `Unit Price` / `Package Size` / `Unit Price Unit`
- `Retail Price` / `Estimated Status` / `Special Status` / `Stock Status`
- `Product URL` / `Run Date`

---

## Project Goal
- Analyze pricing trends, product availability, and category performance.  
- Extract insights for business decisions, such as identifying top-selling products and monthly sales trends.  
- Build dashboards to visualize data and support decision-making.

---

## Key Skills
- **Python** (pandas, matplotlib/seaborn)  
- **SQL** (data aggregation, joins, window functions)  
- **Data Visualization** (Power BI / Tableau)  
- **Analytics & Business Insights**

---

## Project Workflow
1. **Data Cleaning & Exploration**  
   - Remove duplicates, handle missing values, compute new metrics like `TotalSales`.

2. **KPI Calculation**  
   - Total sales, top products, monthly trends, category performance.

3. **SQL Queries**  
   - Aggregate sales, top products, monthly breakdowns.

4. **Dashboard / Visualization**  
   - Create charts & dashboards for sales insights.


---

## Repository Structure
retail-sales-analytics/
├── data/ # Original dataset CSV
├── notebooks/ # Python notebooks
│ └── retail_analysis.ipynb
├── sql/ # SQL queries
│ └── sales_queries.sql
├── dashboard/ # Power BI / Tableau files
│ └── retail_dashboard.pbix
└── README.md

---

## How to Use
1. Clone the repository  
git clone https://github.com/arman690/au-grocery-sales-analysis.git

yaml
Copy code
2. Explore the notebooks to understand data cleaning and analysis  
3. Run SQL queries if using a database  
4. Open dashboard files in Power BI or Tableau for visualization

