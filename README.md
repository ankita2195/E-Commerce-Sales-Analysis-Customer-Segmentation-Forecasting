# E-Commerce Sales, Customer Segmentation & Forecasting Analysis

## Executive Summary

This project analyzes 9,994+ e-commerce transactions to uncover the key drivers of revenue growth, customer retention, and future sales performance. Using exploratory data analysis (EDA), RFM-based customer segmentation, and time series forecasting, the project transforms raw transactional data into actionable business insights.

The analysis identified Technology as the highest revenue-generating category, Office Supplies as the fastest-growing category, and a significant concentration of customers in At Risk and Lost segments, highlighting both growth opportunities and retention challenges. A Holt-Winters forecasting model was developed to estimate future sales demand and support inventory, marketing, and financial planning decisions.

The outcome is a comprehensive set of data-driven recommendations designed to improve customer retention, optimize product strategy, and drive sustainable revenue growth.

---

## Business Problem

E-commerce businesses generate large volumes of transactional data but often struggle to convert that data into strategic decisions.

Key business questions addressed in this project include:

* Which product categories contribute most to revenue and growth?
* Which customers generate the highest long-term value?
* Which customer groups are at risk of churn and require intervention?
* How do sales trends evolve over time?
* What level of sales demand can be expected in the coming months?
* Where should marketing and operational resources be allocated to maximize business impact?

The objective was to create a data-driven framework that enables better decision-making across sales, marketing, inventory management, and customer retention.

---

## Methodology

### 1. Data Preparation & Cleaning

* Processed and cleaned transactional sales data.
* Handled missing values and duplicates.
* Standardized data formats and validated key business metrics.
* Created time-based features for trend and forecasting analysis.

### 2. Exploratory Data Analysis (EDA)

* Analyzed sales performance across categories, products, customers, and regions.
* Examined monthly and yearly revenue trends.
* Identified top-performing and underperforming markets.
* Investigated purchasing patterns and customer behavior.

### 3. RFM Customer Segmentation

Customers were segmented using:

* Recency (How recently a customer purchased)
* Frequency (How often a customer purchases)
* Monetary Value (How much a customer spends)

The analysis categorized customers into actionable business segments such as:

* High-Value
* Loyal
* Potential Loyalists
* At Risk
* Lost
* Dormant High Value
* Churned Loyal
* Churned Frequent

This segmentation enabled targeted retention and marketing strategies.

### 4. Time Series Forecasting

* Aggregated sales at the monthly level.
* Performed an 80/20 train-test split.
* Applied Holt-Winters Exponential Smoothing for forecasting.
* Evaluated performance using RMSE.
* Generated future sales forecasts to support planning and decision-making.

### 5. Business Opportunity Analysis

Combined insights from sales performance, customer segmentation, and forecasting to identify growth opportunities and strategic recommendations.

---

## Skills & Tools

### Programming & Analytics

* Python
* Pandas
* NumPy

### Data Visualization

* Matplotlib
* Seaborn

### Analytics Techiniques

* Exploratory Data Analysis (EDA)
* Customer Segmentation
* RFM Analysis
* Time Series Forecasting
* Sales Trend Analysis
* Business Analytics

---

## Results & Business Recommendations

### Key Findings

#### 1. Product Performance

* Technology generated the highest total revenue ($836K+), demonstrating strong pricing power and high customer value.
* Office Supplies emerged as the fastest-growing category, growing by over 62% between 2014 and 2017.
* Furniture showed steady growth but lagged behind the other categories in overall performance.

#### 2. Customer Segmentation

* At Risk customers represented one of the largest customer groups, indicating significant retention risk.
* Lost customers highlighted substantial customer churn that requires immediate attention.
* High-Value customers contributed disproportionately to revenue and should remain a strategic priority.

#### 3. Sales Forecasting

* Forecast results suggest relatively stable sales performance over the next six months.
* No significant long-term decline was detected.
* Demand fluctuations are expected to continue, reinforcing the need for proactive inventory planning.

### Business Recommendations

#### 1. Expand High-Growth Categories

Increase inventory investment, promotional activity, and product assortment within the Office Supplies category to capitalize on sustained growth momentum.

#### 2. Protect High-Value Customers

Implement VIP loyalty programs, exclusive offers, early-access promotions, and personalized engagement campaigns to maximize customer lifetime value.

#### 3. Reduce Customer Churn

Launch targeted win-back campaigns for At Risk and Lost customers through personalized discounts, reminder emails, and reactivation incentives.

#### 4. Optimize Regional Strategy

Allocate marketing resources toward top-performing markets while investigating barriers limiting performance in underperforming regions.

#### 5. Improve Demand Planning

Utilize forecast outputs to align inventory purchases, staffing decisions, and promotional schedules with anticipated sales demand.

---

## Next Steps & Limitations

### Limitations

* Forecasting was conducted using approximately four years of historical data, limiting the ability to capture longer-term patterns.
* External factors such as economic conditions, competitor actions, holidays, and promotional events were not included in the forecasting model.
* The model focused on sales revenue and did not incorporate profitability or customer acquisition costs.
* Confidence intervals were not included in the final forecast.

### Next Steps

* Implement advanced forecasting models such as SARIMA or Prophet to better capture seasonality.
* Incorporate promotional calendars and holiday effects into forecasting.
* Develop customer lifetime value (CLV) models for deeper retention analysis.
* Build an interactive Power BI dashboard for real-time monitoring.
* Extend the analysis to profitability and margin optimization.
* Create recommendation systems for cross-selling and upselling opportunities.

---

## Repository Structure

```text
├── data/
│   ├── raw_data.csv
│   └── processed_data.csv
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_exploratory_data_analysis.ipynb
│   ├── 03_rfm_segmentation.ipynb
│   ├── 04_time_series_forecasting.ipynb
│   └── 05_business_opportunity_analysis.ipynb
│
├── reports/
│   ├── Business_Report.pdf
│   └── Presentation.pptx
│
├── visualizations/
│   ├── sales_trends.png
│   ├── category_analysis.png
│   ├── rfm_heatmap.png
│   ├── customer_segments.png
│   └── sales_forecast.png
│
├── requirements.txt
└── README.md
```

This project demonstrates how data analytics can move beyond reporting to drive strategic business decisions, helping organizations improve customer retention, optimize operations, and identify scalable growth opportunities.
