# Customer Order Insights

Exploring 99K+ e-commerce orders to uncover customer behaviour, payment trends,
delivery performance, and what drives customer satisfaction.

---

## Project Overview

This project analyses e-commerce order data to better understand customer and
order behaviour.

The main goal was to identify patterns in purchasing activity, payment methods,
delivery performance, and customer satisfaction, and then translate those
findings into practical business insights.

This repository contains **Part 1** of the project, focused on data analysis.

A future **Part 2** will explore machine-learning approaches.

---

## Business Problem

The project focuses on understanding:

- How order activity changes over time
- When customers are most active
- Which payment methods are most commonly used
- How delivery time affects customer satisfaction
- Whether late deliveries are associated with lower review scores

The main business question was:

> How do customer order patterns and delivery performance relate to customer
> satisfaction?

---

## Dataset

The dataset contains approximately **99,000 e-commerce orders**.

It includes information on:

- Order status
- Purchase dates
- Delivery dates
- Number of items
- Product price
- Freight cost
- Payment type
- Installments
- Customer review scores

Each row represents a single order.

---

## Tools & Skills

### Tools

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook

### Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Missing Value Analysis
- Outlier Detection
- KPI Analysis
- Data Visualisation
- Customer & Order Behaviour Analysis
- Statistical Hypothesis Testing
- Business Insight Generation
- Business Recommendations

---

## Approach

The project followed a structured data-analysis workflow:

1. Loaded and inspected the dataset
2. Checked data types, duplicates, and missing values
3. Converted date columns into datetime format
4. Created additional time and delivery features
5. Created a separate delivered-orders dataset
6. Flagged delivery-time outliers using the IQR method
7. Calculated key business KPIs
8. Analysed customer order behaviour
9. Analysed payment behaviour
10. Investigated customer review scores
11. Compared delivery time with customer satisfaction
12. Compared late and on-time deliveries
13. Performed statistical hypothesis testing
14. Developed business insights and recommendations

---

## Key Analysis

### Order Behaviour

Customer activity showed clear time-based patterns.

Orders were highest at the beginning of the week, with **Monday and Tuesday**
showing the strongest activity, while **Saturday** recorded the lowest order
volume.

Order activity was also lowest during the early morning hours and increased
sharply from around **08:00**, remaining high throughout the afternoon and
early evening.

---

### Basket Size

Most orders contained relatively few items.

Single-item purchases represented the typical basket size, suggesting that
customers generally placed smaller rather than large multi-item orders.

---

### Payment Behaviour

Credit cards were the most commonly used payment method by a large margin.

This suggests that reliable card-payment processing plays an important role
in the overall customer purchasing experience.

---

### Delivery Time and Customer Satisfaction

Customer review scores declined as delivery time increased.

Orders delivered more quickly received stronger customer ratings, while longer
delivery periods were associated with lower satisfaction.

---

### Late vs On-Time Deliveries

Delivery reliability produced the strongest finding in the project.

- **On-time orders:** approximately **4.29 stars**
- **Late orders:** approximately **2.57 stars**

Customers whose orders arrived late gave substantially lower review scores.

---

## Statistical Testing

A Welch's independent-samples t-test was used to compare customer review scores
between late and on-time deliveries.

The result showed a statistically significant difference between the two groups.

This provides further evidence that late delivery is strongly associated with
lower customer satisfaction.

The result shows association and should not be interpreted as proof that late
delivery is the only cause of lower customer ratings.

---

## Key Findings

The main findings from the project were:

- Delivery reliability is strongly associated with customer satisfaction.
- Late deliveries received much lower average review scores.
- Customer satisfaction declined as delivery time increased.
- Credit cards were the dominant payment method.
- Most orders contained relatively few items.
- Customer order activity varied by month, day of week, and hour of day.

---

## Business Recommendations

Based on the analysis, the business should:

- Prioritise improving on-time delivery performance.
- Monitor orders approaching their estimated delivery date.
- Investigate unusually long delivery times for operational issues.
- Use purchasing patterns by day and hour to support staffing and planning.
- Maintain reliable credit-card payment infrastructure.

---

## Project Structure

```text
customer-order-insights/
│
├── README.md
├── Customer_Behaviour_Analysis_Project.ipynb
├── data/
│   └── orders.csv
└── outputs/
    └── customer_orders_cleaned.csv
