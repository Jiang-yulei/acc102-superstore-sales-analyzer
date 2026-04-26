# Superstore Sales Analyzer

## 1. Problem & Target User
**Problem:** Store managers need a quick, multi‑dimensional overview of sales and profit performance.  
**Target User:** Supermarket store managers, retail operations analysts.

## 2. Dataset
- **Source:** Kaggle – [Superstore Sales by Ishan Shrivastava](https://www.kaggle.com/datasets/ishanshrivastava28/superstore-sales)
- **Access Date:** 20 April 2026
- **Key Fields:** Order Date, Category, Sub‑Category, Sales, Profit, Region

## 3. Methods (Python steps)
1. Load CSV with `pandas`.
2. Clean data: convert `Sales`, `Profit` to numeric, `Order Date` to datetime, drop missing values.
3. Extract month for time series.
4. Generate 7 visualisations and print key business insights (dynamic, using `idxmax()`, quartiles, etc.):
   - Sales by Category (bar)
   - Profit by Category (bar)
   - Sales Share by Category (pie)
   - Sales by Region (bar)
   - Monthly Sales Trend (line)
   - Sales vs Profit Scatter (per transaction)
   - Top 10 Sub‑Categories by Sales (horizontal bar)
      
## 4. Key Findings
- **Best‑selling and most profitable category:** Technology    
- **Top region:** West (≈$450k)  
- **Top sub‑category:** Phones (≈$200k)    
- **Monthly trend:** peak months (e.g., April 2015) and low months (e.g., December 2014).  
- 18.7% of transactions have negative profit; among medium‑sales ($17–$210), 14.7% are unprofitable.

## 5. How to Run
1. Clone this repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Place the CSV file (`Superstore.csv`) in the same folder as the notebook.
4. Run `ACC102 Superstore Sales Analyzer.ipynb` (Jupyter Notebook) – all cells will produce 7 charts and printed insights.

## 6. Demo Video
[Click here for the demo video](https://www.capcut.cn/share/7633030934912259352?t=1) 

## 7. Limitations & Next Steps
- No cost per unit → cannot calculate profit margin.  
- Data from a single fictional retailer → limited generalisability.  
- Future: add linear regression forecast, build interactive Streamlit dashboard, include profit margin by sub‑category.
