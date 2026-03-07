# 🛒 E-commerce Analytics (PySpark)

This project showcases an end-to-end **data analysis pipeline** for large-scale e-commerce data using **PySpark**.  
It demonstrates advanced analytical workflows commonly used in real-world data engineering and analytics environments — including RFM segmentation, retention analysis, LTV modeling, and funnel conversion tracking.

---

## 📊 Project Overview

The goal of this project is to analyze a large (2 GB) e-commerce dataset and extract actionable business insights by leveraging the scalability of **Apache Spark**.

Key analyses include:
- **Category performance analysis** (orders, revenue)
- **RFM segmentation** to identify customer groups (Champions, At Risk, etc.)
- **Cohort retention** by first purchase date
- **LTV (Customer Lifetime Value)** estimation
- **Conversion funnel** from view → cart → purchase
- **Market basket analysis** (co-purchased product pairs)

---

## ⚙️ Tech Stack

| Tool / Library | Purpose |
|-----------------|----------|
| **PySpark (Spark SQL, DataFrame API)** | Large-scale data processing |
| **Databricks** | Interactive execution environment |
| **SQL** | Data extraction and transformation |

---

## 🧠 Main Insights

- RFM segmentation revealed that **15% of users ("Champions") generate over 60% of revenue**.  
- Customer retention sharply drops after day 7 — suggesting the need for **early re-engagement campaigns**.  
- Conversion funnel shows **only ~6% of product views lead to purchase**.  
- Market basket analysis identified strong associations between products in **electronics** and **accessories** categories.

---

## 🧩 Project Structure

```
ecommerce-analytics-pyspark/
│
├── notebooks/
│   └── ecommerce_analysis.ipynb        # main exploratory notebook
│
├── README.md
└── requirements.txt
```

---

## 🚀 How to Run

### Option 1: Databricks (recommended)
1. Upload `ecommerce_analysis.py` or `.ipynb` to your Databricks workspace.
2. Attach a cluster with Spark 3.x.
3. Run all cells or submit as a job.
4. View visual outputs using `display()` in Databricks notebooks.

### Option 2: Local PySpark
```bash
pip install pyspark
python scripts/ecommerce_analysis.py
```

---

## 📚 Future Improvements

- Integrate automated report generation with Power BI or Streamlit  
- Add predictive LTV modeling (XGBoost, regression)  
- Implement Airflow DAG for data pipeline scheduling  

---

## 👤 Author

**Tomasz Cielepak**  

---

