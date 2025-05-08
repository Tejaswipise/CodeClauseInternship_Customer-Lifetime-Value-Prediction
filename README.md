# CodeClauseInternship_Customer-Lifetime-Value-Prediction

## Customer Lifetime Value (CLV) Prediction Report



## Table of Contents:
- [Introduction](#1-introduction)
- [Problem Definition](#2-problem-definition)
- [Data Source](#3-data-source)
- [Approach and Methodology](#4-approach-and-methodology)
- [Key Insights and Findings](#5-key-insights-and-findings)
- [Conclusion](#6-conclusion)
- [Future Work](#7-future-work)

## 1. Introduction

In today’s competitive e-commerce landscape, understanding and predicting **Customer Lifetime Value (CLV)** is crucial. CLV helps businesses understand the total revenue a customer is likely to generate over their entire relationship with the company. This information can guide businesses in crafting targeted marketing strategies, improving customer service, and boosting customer retention. The goal of this project was to predict CLV for customers based on past purchasing behaviors and gain insights into how to engage with high-value customers more effectively.

## 2. Problem Definition

The core problem we are tackling is predicting the **Customer Lifetime Value (CLV)** for an e-commerce platform (Olist). Knowing the CLV of customers allows the business to identify which customers are most likely to generate long-term revenue, which helps in targeting marketing efforts and improving customer retention. By predicting CLV, businesses can adjust their strategies and resources accordingly, ensuring they spend on the right customers.

## 3. Data Source

For this project, we used the **Brazilian E-Commerce Public Dataset by Olist**. This dataset provides a detailed snapshot of transactions on the Olist platform, including data on customers, orders, products, payments, and reviews. The data consists of the following files:

* **olist\_customers\_dataset.csv**: Contains information about customers (e.g., demographics, location).
* **olist\_geolocation\_dataset.csv**: Provides geographical data for customers and sellers.
* **olist\_orders\_dataset.csv**: Details about each order placed by customers.
* **olist\_order\_items\_dataset.csv**: Information about items purchased in each order.
* **olist\_order\_payments\_dataset.csv**: Payment details for each order.
* **olist\_order\_reviews\_dataset.csv**: Customer feedback and reviews for orders.
* **olist\_products\_dataset.csv**: Product details (categories, descriptions).
* **olist\_sellers\_dataset.csv**: Information about sellers.
* **product\_category\_name\_translation.csv**: Translations of product categories into English.

This rich dataset allowed us to analyze customer behavior and predict their future value.

## **4. Approach and Methodology**

The process was carried out in several key steps to ensure comprehensive insights and actionable outcomes:

### **Step 1: Data Preprocessing and Cleaning**

We started by exploring the dataset to understand its structure and relationships between different variables. The data was cleaned by:

* Handling **missing values** and standardizing data formats.
* Identifying and dealing with **outliers** that could distort our results.
* Ensuring all variables were in the right format for analysis.

### **Step 2: Feature Engineering**

Feature engineering was crucial for preparing the data for modeling. Key metrics like **Recency**, **Frequency**, and **Monetary (RFM)** were calculated for each customer:

* **Recency**: How recent was the customer’s last purchase?
* **Frequency**: How often does the customer make a purchase?
* **Monetary**: How much has the customer spent overall?

We also calculated **Customer Tenure** (how long each customer has been interacting with the platform) and segmented customers into "one-time buyers" and "repeated buyers." This segmentation helped categorize the customer base more clearly.

### **Step 3: Customer Segmentation**

Using the RFM metrics, we divided customers into various segments. This segmentation was done using **K-means clustering**, which grouped customers based on their purchasing patterns. These segments helped us understand which customers were high-value, which were likely to churn, and which were more cost-effective to target.

### **Step 4: Predictive Modeling for CLV**

Once the features were ready, we built a regression model to predict **total CLV** and **future CLV** for each customer. We used algorithms like **Linear Regression** and **Random Forest** to create the prediction models.

### **Step 5: Churn Analysis**

We analyzed **churn rates** across customer segments. This helped us understand which customers were at risk of leaving and which were more loyal. By understanding churn, we could identify the customers we should focus on for retention campaigns.

## **5. Key Insights and Findings**

1. **RFM Segmentation**: Customers with high **frequency** and **monetary** scores were identified as high-value customers. These customers are likely to contribute more to long-term revenue.

2. **K-means Clustering**: The clustering results helped segment customers based on their RFM scores, giving us a clear picture of high-value versus low-value customers. This insight is key for marketing teams to tailor strategies for each segment.

3. **Feature Importance**: The **monetary value** of a customer emerged as the most significant predictor of their lifetime value, followed closely by their **frequency of purchase**.

4. **Churn Rate**: Our churn analysis showed that customers with low-frequency purchases and lower spending had higher churn rates. This suggests that businesses should focus on engaging these customers before they churn.

## **6. Conclusion **

The project successfully identified high-value customers and those at risk of churning using various data science techniques. Here are a few recommendations:

* **Focus on High-Value Customers**: Target customers with high frequency and high monetary value for personalized marketing campaigns to boost their CLV.
* **Engage Low-Frequency Customers**: Consider running re-engagement campaigns targeting customers who purchase infrequently but show potential for higher value.
* **Churn Prevention**: Keep a close eye on customer segments that have a high churn risk. Offer them special promotions or personalized services to increase retention.

The insights gathered from the RFM analysis, customer segmentation, and churn analysis can help businesses better allocate marketing resources and improve customer relationships.

## **7. Future Work**

While the current model offers useful predictions for CLV, there is potential for improvement:

* **Advanced Machine Learning Models**: We can explore more sophisticated models, such as **XGBoost** or **Deep Learning** models, for better accuracy in CLV predictions.
* **Real-Time CLV Prediction**: Implementing a dynamic CLV prediction system that adjusts in real time as new customer data is collected could enhance customer engagement strategies.


