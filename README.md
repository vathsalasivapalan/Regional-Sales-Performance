# 📊 Regional Sales Performance Analysis

An end-to-end sales data analysis project for XYZ Co. covering 2014–2018,
exploring revenue drivers, regional trends, channel performance, and 
budget vs actuals using Python and Power BI.

---

## 📌 Problem Statement

Analyze XYZ Co.'s sales data from 2014–2018 to identify key revenue and 
profit drivers across products, channels, and regions. Uncover seasonal 
trends and outliers, and evaluate performance against budget targets. 
Use these insights to optimize pricing strategies, promotional activities, 
and market expansion efforts to achieve sustainable growth and reduce 
concentration risk.

---

## 🛠️ Tools Used

- **Python** — Data cleaning, merging, feature engineering, EDA
- **Pandas & NumPy** — Data manipulation and analysis
- **Matplotlib & Seaborn** — Data visualisation
- **Power BI** — Interactive dashboard and reporting
- **OpenPyXL** — Reading multi-sheet Excel files

---

## 📂 Dataset

- **Source:** XYZ Co. Internal Sales Dataset (Regional Sales Dataset.xlsx)
- **Records:** 64,104 orders across 6 merged sheets
- **Period:** January 2014 – December 2018
- **Sheets merged:**
  - `Sales Orders` — core transaction data
  - `Customers` — customer name lookup
  - `Products` — product name lookup
  - `Regions` — geographic data (state, county, population, median income)
  - `State Regions` — maps states to US regions
  - `2017 Budgets` — budget targets by product

- **Key Columns:**

| Column | Description |
|--------|-------------|
| `OrderDate` | Date of order (2014–2018) |
| `Channel` | Sales channel — Wholesale, Distributor, Export |
| `Region` | US region — South, Midwest, West, Northeast |
| `Product Name` | Product sold |
| `Order Quantity` | Units ordered |
| `Unit Price` | Price per unit |
| `Line Total` | Total revenue per order line |
| `Total Unit Cost` | Cost per unit |
| `2017 Budgets` | Budget target per product for 2017 |
| `median_income` | Median income of delivery region |
| `population` | Population of delivery region |

---

## 🔧 Data Cleaning & Feature Engineering

- Merged 6 Excel sheets into a single master dataframe (64,104 rows × 35 cols)
- Dropped redundant index/lookup columns (reduced to 28 columns)
- Converted high-cardinality string columns to `category` dtype
- Reduced memory usage from **~17.1 MB to ~13.7 MB**
- Confirmed **zero duplicates** and **zero missing values**

---

## 🔍 Key Analysis Areas

- Revenue and profit trends by year (2014–2018)
- Regional performance comparison (South, Midwest, West, Northeast)
- Sales channel breakdown (Wholesale vs Distributor vs Export)
- Product-level performance and top sellers
- 2017 budget vs actual sales comparison
- Geographic analysis using population and median income data

---

## 💡 How to Use

1. Clone the repository
2. Place `Regional Sales Dataset.xlsx` in a `/data` folder
3. Open `reginal_sales_analysis.ipynb` in Jupyter Notebook
4. Run all cells to reproduce the analysis
5. Open `dashboard.pbix` in Power BI Desktop to explore the dashboard

---

## 📁 Project Structure

Regional-Sales-Performance/
│
├── data/
│   └── Regional Sales Dataset.xlsx
├── reginal_sales_analysis.ipynb
├── dashboard.pbix
├── dashboard.pdf
└── README.md

---

## 👤 Author

**Vathsala Sivapalan**  
[GitHub](https://github.com/vathsalasivapalan)
