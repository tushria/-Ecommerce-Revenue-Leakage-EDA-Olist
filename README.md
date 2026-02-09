#### E-Commerce Revenue Leakage & Customer Behavior Analysis (Olist)
#### Exploratory Data Analysis to identify revenue loss drivers such as order cancellations, delayed deliveries, payment failures, and customer behavior patterns.
#### Why This Dataset?
#### Although the dataset is from a Brazilian e-commerce platform, the business challenges analyzed in this project are common to global e-commerce companies, making the insights broadly applicable.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### -- Problem Statement:
#### -- The objective of this project is to analyze real-world e-commerce transactional data to identify revenue leakage drivers such as order cancellations, returns, payment failures, delivery delays, and customer behavior patterns, and to provide actionable business recommendations.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# 📦 E-commerce Order Delivery & Customer Behavior Analysis

## 📌 Project Overview

This project performs an end-to-end Exploratory Data Analysis (EDA) on an e-commerce **orders dataset (99k+ records)** to evaluate **order fulfillment efficiency, delivery performance, and customer behavior**.

The analysis focuses on the complete **order lifecycle** — from purchase to final delivery — with the goal of identifying **logistics bottlenecks, late delivery risks, and retention opportunities**.

This project is designed to closely resemble **real-world data engineering and analytics workflows**, including data cleaning, feature engineering, and business-focused insights.

---

## 🎯 Business Objectives

* Analyze order fulfillment success and failure rates
* Measure delivery speed and identify delay patterns
* Evaluate late delivery performance vs estimated timelines
* Understand time-based demand trends
* Study customer retention and repeat purchase behavior
* Provide actionable business recommendations

---

## 🗂 Dataset Description

**Table Used:** Orders Table
**Records:** 99,441 orders
**Key Columns:**

* `order_id`
* `customer_id`
* `order_status`
* `order_purchase_timestamp`
* `order_approved_at`
* `order_delivered_carrier_date`
* `order_delivered_customer_date`
* `order_estimated_delivery_date`

---

## 🧹 Step 1: Data Cleaning & Preparation

Key actions performed:

* Converted timestamp columns from object to datetime
* Analyzed and retained missing values representing incomplete order lifecycles
* Removed duplicate records
* Standardized column naming conventions
* Removed logically invalid records (negative delivery durations)

### Feature Engineering:

* `delivery_time_days`
* `shipping_delay_days`
* `is_late_delivery`
* `delivery_success`
* `delivery_speed`

---

## 🔄 Step 2: Order Funnel Analysis

Analyzed the progression of orders across lifecycle stages:

* Total orders placed
* Delivered vs canceled/unavailable orders
* Delivery success rate

**Outcome:**

* Identified operational leakage points before final delivery

---

## 🚚 Step 3: Delivery Time & Delay Analysis

* Calculated average, median, and extreme delivery times
* Identified long-tail delivery delays (top 5% orders)
* Segmented delivery speeds into business-friendly categories

**Insight:**

* Majority of orders are delivered within reasonable timelines, but extreme delays pose operational risk

---

## ⏰ Step 4: Late Delivery vs Estimated Date Analysis

* Compared actual delivery dates with estimated delivery dates
* Calculated late delivery rate (only for delivered orders)
* Measured delay severity in days

**Insight:**

* A significant portion of orders miss promised delivery timelines

---

## 📈 Step 5: Time-Based Trends Analysis

* Monthly order volume trends (seasonality)
* Average delivery time trends over time
* Late delivery trend by month
* Orders by weekday and hour (peak demand analysis)

**Insight:**

* Clear seasonality and peak ordering hours observed

---

## 👥 Step 6: Customer Behavior & Retention Analysis

* Segmented customers into one-time vs repeat buyers
* Analyzed delivery performance by customer type
* Studied time gaps between repeat purchases

**Insight:**

* Repeat customers experience better delivery performance
* Late deliveries negatively impact retention

---

## 🧠 Executive Summary

This analysis highlights that while overall delivery success is strong, **logistics inefficiencies, late deliveries, and long-tail delays** significantly impact customer experience. Improving delivery estimation accuracy and prioritizing high-value customers can substantially improve retention and satisfaction.

---

## 💡 Business Recommendations

* Improve delivery date estimation using historical delay data
* Monitor and reduce long-tail delivery delays
* Optimize logistics capacity during peak demand periods
* Prioritize repeat customers for faster fulfillment

---

## 🛠 Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib / Seaborn
* Jupyter Notebook

---

## 📌 Key Skills Demonstrated

* Data Cleaning & Feature Engineering
* Time-series Analysis
* Business-focused EDA
* Customer Retention Analysis
* Logistics & Operations Analytics

---

## 📄 How to Use This Repository

1. Clone the repository
2. Open the Jupyter Notebook
3. Run cells sequentially to reproduce the analysis

---

## 👤 Author

**Sakshi Saini**
Aspiring Data Engineer | Data Analytics | SQL | Python

---

⭐ If you find this project useful, feel free to star the repository!
