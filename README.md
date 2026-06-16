# 🛒 E-Commerce Sales, Customer Segmentation & Forecasting Analysis

## 📊 Executive Summary

This project analyzes 9,994+ e-commerce transactions to uncover the key drivers of revenue growth, customer retention, and future sales performance. Using exploratory data analysis (EDA), RFM-based customer segmentation, and time series forecasting, the project transforms raw transactional data into actionable business insights.

The analysis identified Technology as the highest revenue-generating category, Office Supplies as the fastest-growing category, and a significant concentration of customers in At Risk and Lost segments, highlighting both growth opportunities and retention challenges. A Holt-Winters forecasting model was developed to estimate future sales demand and support inventory, marketing, and financial planning decisions.

The outcome is a comprehensive set of data-driven recommendations designed to improve customer retention, optimize product strategy, and drive sustainable revenue growth.

---

## 🎯 Business Problem

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

## 🔍 Methodology

### 1. Data Preparation & Cleaning

* Processed and cleaned transactional sales data.
* Handled missing values and duplicates. (The data had no duplicate or null values)
* Standardized data formats and corrected the data types.
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

* High-Value- Recently active customers with high purchase frequency and spending.
* Loyal- Consistent repeat customers who regularly engage with the business.
* Potential Loyalists- Customers showing early signs of becoming loyal buyers.
* At Risk- Previously active customers whose engagement has declined significantly.
* Lost- Customers who have not made a purchase for a long period and are likely churned.
* Dormant High Value- High-spending customers who have become inactive. 
* Churned Loyal- Previously loyal customers who have stopped purchasing.
* Churned Frequent- Previously frequent buyers who have become inactive.
* New- Recently acquired customers with limited purchase history.
* Other- Customers who do not clearly fit into any major behavioral segment.

This segmentation enabled targeted retention and marketing strategies.

<img width="525" height="350" alt="segment_distribution" src="https://github.com/user-attachments/assets/ce25bfe7-bb3c-4428-8007-c041e81a3228" />


### 4. Time Series Forecasting

* Aggregated sales at the monthly level.
* Performed an 80/20 train-test split.
* Applied Holt-Winters Exponential Smoothing for forecasting.
* Evaluated performance using RMSE.
* Generated future sales forecasts to support planning and decision-making.

<img width="538" height="300" alt="image" src="https://github.com/user-attachments/assets/6d2b4243-4456-4164-95ab-09c731059c50" />


### 5. Business Opportunity Analysis

Combined insights from sales performance, customer segmentation, and forecasting to identify growth opportunities and strategic recommendations.

---

## 🛠️ Skills & Tools

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

## 📈 Results & Business Recommendations

### 💡 Key Findings

#### 1. Product Performance

* Technology generated the highest total revenue ($836K+), demonstrating strong pricing power and high customer value.
* Office Supplies emerged as the fastest-growing category, growing by over 62% between 2014 and 2017.
* Furniture showed steady growth but lagged behind the other categories in overall performance.

<img width="586" height="350" alt="sales_and_qty_by_category" src="https://github.com/user-attachments/assets/55c554d1-a0a9-4535-9428-59426ab64a68" />

#### 2. Regional Performance

- New York, Los Angeles, and Seattle emerged as the strongest-performing markets, consistently contributing high sales volumes and revenue.
- Several cities such as Abilene, Elyria, and Jupiter showed minimal sales activity, indicating opportunities to investigate market penetration, customer demand, and distribution challenges.
- Geographic sales concentration suggests that targeted regional marketing and inventory allocation can further improve revenue performance.

#### 3. Customer Segmentation

* At Risk customers represented one of the largest customer groups, indicating significant retention risk.
* Lost customers highlighted substantial customer churn that requires immediate attention.
* High-Value customers contributed disproportionately to revenue and should remain a strategic priority.

#### 4. Sales Forecasting

* Forecast results suggest relatively stable sales performance over the next six months.
* No significant long-term decline was detected.
* Demand fluctuations are expected to continue, reinforcing the need for proactive inventory planning.

<img width="564" height="300" alt="6-month predictions" src="https://github.com/user-attachments/assets/e7de5d9c-ff71-4e6b-9b3c-a425dcebca5c" />

### 🚀 Business Recommendations

#### 1. Expand High-Growth Categories

Increase inventory investment, promotional activity, and product range within the Office Supplies category to capitalize on sustained growth.

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

### ⚠️ Limitations

* Forecasting was conducted using approximately four years of historical data, limiting the ability to capture longer-term patterns.
* External factors such as economic conditions, competitor actions, holidays, and promotional events were not included in the forecasting model.
* The model focused on sales revenue and did not include profitability or customer acquisition costs.
* Confidence intervals were not included in the final forecast.

### 🔮 Next Steps

* Implement advanced forecasting models such as SARIMA or Prophet for more accurate forecasting.
* Include promotional calendars and holiday effects into forecasting.
* Develop customer lifetime value (CLV) models for deeper retention analysis.
* Build an interactive Power BI dashboard for real-time monitoring.
* Extend the analysis to profitability and margin optimization.
* Create recommendation systems for cross-selling and upselling opportunities.

---

## 📂 Repository Structure

```text
├── data/
├── notebook/
├── report and presentation/
│   ├── Business_Report.pdf
│   └── Presentation.pptx
│
├── visualizations/
└── README.md
```

This project demonstrates how data analytics can move beyond reporting to drive strategic business decisions, helping organizations improve customer retention, optimize operations, and identify scalable growth opportunities.
