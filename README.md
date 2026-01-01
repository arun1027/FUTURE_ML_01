# Sales Forecasting and Visualization using Prophet & Power BI

## Overview
This project focuses on analyzing historical sales data and generating **time series forecasts** using the **Facebook Prophet** model. The forecasted results are visualized using **Power BI** to deliver clear, actionable business insights.

The objective is to understand sales trends, seasonality, and future demand to support data-driven decision-making.

---

## Dataset
- **Source:** Adidas US Sales Dataset  
- **Format:** Excel (`.xlsx`)
- **Granularity:** Daily sales data  
- **Key fields:**
  - Invoice Date
  - Category
  - Region / Store
  - Total Sales

Raw data is stored separately from processed data to ensure reproducibility.

---

## Project Structure
```text
sales-forecasting/
│
├── data/
│   ├── raw/
│   │   └── Adidas_US_Sales_Dataset.xlsx
│   ├── forecast/
│   │   └── sales_forecast.csv
│
├── notebooks/
│   └── Sales_Prediction.ipynb
│
├── powerbi/
│   └── ML_INTERN_TASK_1.pbix
│
├── README.md
└── requirements.txt
```

---

## Methodology

### 1. Data Preprocessing
- Converted date columns to datetime format
- Aggregated sales at the **daily level**
- Handled missing values and inconsistencies

### 2. Time Series Forecasting
- Used **Prophet** for forecasting
- Modeled trend and seasonality
- Generated future predictions using `make_future_dataframe`
- Evaluated model using MAE and MSE

### 3. Visualization
- Exported forecast results to CSV
- Built an interactive **Power BI dashboard**

---

## Power BI Dashboard Features
- Actual vs Forecasted sales trend
- Monthly and yearly comparisons
- Filters by category, store, and region
- Identification of top-selling categories and low-sales periods
- Insight cards for business decision-making

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Prophet
- Scikit-learn
- Power BI
- Jupyter Notebook

---

## How to Run the Project
1. Clone the repository  
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:
    ```bash
    notebooks/Sales_Prediction.ipynb
    ```
4. Load the processed file into Power BI:
    ```bash
    data/processed/sales_forecast.csv
    ```

---

## Results & Insights
- Identified clear sales trends and seasonality patterns  
- Generated short-term forecasts to support planning and decision-making  
- Daily forecasts provide granular insights, while aggregation improves stability  
- Forecast comparison highlights gaps between expected and actual performance  

---

## Conclusion
This project demonstrates an **end-to-end time series forecasting workflow**, covering data preprocessing, modeling with Prophet, and visualization using Power BI. The analysis provides actionable insights into sales trends and future demand, supporting data-driven business decisions. The approach can be further enhanced by incorporating holidays, promotions, or external regressors.

---
## Author
Arun Natarajan

