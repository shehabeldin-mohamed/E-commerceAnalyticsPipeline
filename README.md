# E-Commerce Big Data Analytics Pipeline

A robust data engineering workflow designed to handle and analyze over **67 million rows** of e-commerce behavior data. This project demonstrates the transition from raw, unoptimized logs to structured PostgreSQL storage and business visualizations.

## Project Overview
The primary goal of this project was to engineer a scalable solution for processing massive e-commerce datasets. By leveraging **Apache Spark**, the pipeline addresses common "big data" challenges such as schema inconsistencies, massive null counts, and data redundancy.

## Tech Stack
* **Engine:** Apache Spark (PySpark)
* **Storage:** PostgreSQL
* **Analysis:** Pandas, SQL
* **Visualization:** Matplotlib, Seaborn

## Key Features & Workflow

### 1. Data Cleaning & Optimization
* **Scale:** Successfully processed 67M+ records of raw e-commerce event logs.
* **Integrity:** Implemented programmatic logic to handle significant null values, remove duplicates, and standardize schema inconsistencies.
* **Schema Enforcement:** Defined strict data types for event timestamps and price values to optimize memory usage and ensure data reliability.

### 2. Transformation & Storage
* **Aggregations:** Built complex Spark transformations to calculate daily traffic (Visits/Visitors), total revenue, and daily conversion rates.
* **Persistence:** Optimized the cleaned dataset and persisted it into a **PostgreSQL** database, creating a reliable foundation for downstream BI tools.

### 3. Analytics & Visualization
* **Data Bridge:** Converted specific Spark aggregation outputs to Pandas to enable localized, high-performance visualization.

---

## Insights & Visualizations

### Daily Visits & Daily Visits By Day
This chart illustrates the number of daily visits. Note the significant spike during the mid-month promotional events (Black Friday period).

![Daily Visits](Visuals/daily_visits_combined.png)

### Conversion Rate Performance
By analyzing the ratio of purchases to visits, we can identify "high-quality" traffic days. The data reveals that the mid-month surge was accompanied by a nearly triple increase in conversion efficiency.

![Conversion Rates](Visuals/daily_conversion_combined.png)

### Daily Visitors & Daily Visitors By Day
The plots illustrates the number of daily visitors. Here you can also see the significant spike during the mid-month promotional events (Black Friday period).

![Daily Visitors](Visuals/daily_visitors_combined.png)

---
## Data Source & Disclaimer

The dataset used in this project is available on [Kaggle](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store/data).

This project is created **for educational purposes only**. I do not claim ownership of the dataset.

If you are the data owner and would like this dataset or project removed or modified, please reach out via an issue or message.

---
Feel free to explore the google colab notebook to see the other plots, and the cleaning process.
