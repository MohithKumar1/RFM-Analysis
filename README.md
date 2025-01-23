# RFM-Analysis project

This project performs Recency, Frequency, and Monetary (RFM) analysis on a retail dataset to segment customers into distinct value categories based on their purchasing behavior. It leverages Python libraries such as Pandas for data manipulation and Excel integration.

# Project Overview
The goal of this project is to segment customers into three value-based classes:

High Value
Medium Value
Low Value
This segmentation is based on customers' purchase recency, frequency, and monetary contributions using the RFM framework.

# Key Questions Answered:

How recently has a customer made a purchase? (Recency)
How often does the customer make purchases? (Frequency)
How much does the customer spend? (Monetary)

# Dataset
The dataset used for this project is OnlineRetail.xlsx, which contains the following columns:

InvoiceNo: Unique invoice identifier.
StockCode: Unique product code.
Description: Description of the product.
Quantity: Number of units sold.
InvoiceDate: Date of transaction.
UnitPrice: Price per unit.
CustomerID: Unique customer identifier.
Country: Country of purchase.

# Key Features

1.Data Cleaning and Preprocessing
  Removed null values to ensure data integrity.
  Converted the InvoiceDate column to datetime format.
  Derived new columns like Total_value (calculated as Quantity * UnitPrice).
2.RFM Metric Calculation
  Recency: Days since the last purchase for each customer.
  Frequency: Total number of purchases per customer.
  Monetary: Total spending of each customer.
3.RFM Segmentation
  1.Normalized RFM ranks into percentages for fair comparison.
  2.Calculated an overall RFM score using weighted contributions:
    Recency: 15%
    Frequency: 28%
    Monetary: 57%
  3.Classified customers into:
    High Value: RFM score > 75
    Medium Value: RFM score ≤ 75 and > 25
    Low Value: RFM score ≤ 25

# Key Findings:
  High-Value Customers: Customers with RFM scores above 75 contribute significantly to the business's revenue.
  Medium-Value Customers: Customers with moderate purchase behavior, potentially convertible to high-value.
  Low-Value Customers: Customers who have minimal interactions, requiring retention strategies.

# Applications:
  Customer Retention: Focus on high-value customers to maintain loyalty.
  Upselling and Cross-Selling: Target medium-value customers with personalized offers.
  Reactivation Campaigns: Engage low-value customers with discounts or reminders.


