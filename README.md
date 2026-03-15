# Customer Segmentation using RFM Analysis & K-Means Clustering

## Project Overview
Understanding customer behavior is essential for businesses to improve marketing strategies and increase revenue.  
This project performs **customer segmentation using RFM (Recency, Frequency, Monetary) analysis and K-Means clustering** to identify high-value customers, loyal customers, and customers at risk of churn.

By analyzing historical transaction data, the project uncovers **distinct customer groups and actionable insights** that can support targeted marketing and customer retention strategies.


## Business Objective
The goal of this project is to segment customers based on their purchasing behavior in order to:

- Identify **high-value customers contributing most revenue**
- Detect **customers at risk of churn**
- Understand **purchasing patterns and engagement levels**
- Enable **data-driven marketing strategies**


## Dataset
The analysis uses the **Online Retail dataset**, which contains transaction-level data from an e-commerce store.

### Dataset Features

| Feature | Description |
|--------|-------------|
| InvoiceNo | Unique transaction ID |
| StockCode | Product identifier |
| Description | Product name |
| Quantity | Number of items purchased |
| InvoiceDate | Date of purchase |
| UnitPrice | Price of each item |
| CustomerID | Unique customer identifier |
| Country | Customer location |

Dataset size: **~500,000 transactions**


## Methodology

### 1. Data Cleaning
- Removed missing customer IDs
- Removed cancelled transactions
- Converted date fields to datetime format
- Calculated total transaction value

### 2. Feature Engineering (RFM Analysis)
Customer behavior was analyzed using **RFM metrics**:

| Metric | Description |
|------|-------------|
| Recency | Days since last purchase |
| Frequency | Number of purchases |
| Monetary | Total spending by the customer |

These metrics capture **customer engagement and value**.


### 3. Data Normalization
RFM features were standardized using **StandardScaler** to ensure equal importance during clustering.


### 4. Customer Segmentation using K-Means
The **K-Means clustering algorithm** was used to group customers with similar purchasing behaviors.

The **Elbow Method** was applied to determine the optimal number of clusters.

Customers were segmented into behavioral groups such as:

- **Champions** – High spending and frequent buyers
- **Loyal Customers** – Consistent repeat buyers
- **Regular Customers** – Moderate purchasing behavior
- **At-Risk Customers** – Customers who have not purchased recently


## Key Insights

- A small percentage of customers contribute **a large share of total revenue**.
- Loyal customers exhibit **high purchase frequency and consistent engagement**.
- At-risk customers previously showed purchasing activity but have **not purchased recently**, indicating potential churn.
- Targeted marketing campaigns can significantly improve **customer retention and lifetime value**.


## Business Recommendations

| Segment | Strategy |
|--------|----------|
| Champions | Offer loyalty rewards and premium benefits |
| Loyal Customers | Encourage repeat purchases through personalized promotions |
| Regular Customers | Upsell products and targeted offers |
| At-Risk Customers | Launch re-engagement campaigns |


## Key Metrics

| Metric | Value |
|------|------|
| Transactions Analyzed | 500,000+ |
| Customers Segmented | 4,000+ |
| Segments Identified | 4 |
| Revenue Share of Top Segment | ~60% |



## Tools & Technologies
- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib / Seaborn**
- **Jupyter Notebook**

## Analytics Pipeline

Data Cleaning → RFM Feature Engineering → Data Scaling → K-Means Clustering → Segment Profiling → Business Insights


## Conclusion
This project demonstrates how **customer segmentation using machine learning techniques** can uncover valuable insights into customer behavior.  
Businesses can leverage these insights to design **data-driven marketing strategies**, improve **customer retention**, and increase **overall revenue performance**.
