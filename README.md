# Exploratory Data Analysis (EDA)

## Project Overview

This project performs an Exploratory Data Analysis of an e-commerce order dataset using Microsoft Excel. The analysis focuses on descriptive statistics, daily sales and order trends, IQR-based outlier detection, and the main observations identified from the data.

The workbook contains 1,200 orders with 14 variables covering order information, customer and product details, quantities, prices, cart contents, payment methods, order status, promotions, referral sources, and total prices.

## Objectives

- Summarize the main numerical variables using count, mean, median, minimum, and maximum values.
- Examine daily order activity, sales, and quantity.
- Identify daily sales highs and lows.
- Detect potential outliers using the IQR method.
- Investigate the identified outliers and determine their relevance to the analysis.
- Summarize the main observations and patterns found in the dataset.

## Dataset

The Dataset worksheet contains 1,200 rows and 14 columns.

The variables analyzed include:

- OrderID
- Date
- CustomerID
- Product
- Quantity
- UnitPrice
- ShippingAddress
- PaymentMethod
- OrderStatus
- TrackingNumber
- ItemsInCart
- CouponCode
- ReferralSource
- TotalPrice

The order dates range from January 1, 2023 to June 30, 2025.

The workbook's numerical analysis focuses on Quantity, UnitPrice, ItemsInCart, and TotalPrice.

## Analysis Performed

### Basic Statistics

The Basic Statistics worksheet calculates the count, mean, median, minimum, and maximum for the four numerical variables:

| Variable | Count | Mean | Median | Min | Max |
|---|---:|---:|---:|---:|---:|
| Quantity | 1,200 | 2.95 | 3.00 | 1 | 5 |
| UnitPrice | 1,200 | 356.41 | 364.21 | 11.39 | 699.93 |
| ItemsInCart | 1,200 | 5.49 | 5.00 | 1 | 10 |
| TotalPrice | 1,200 | 1,053.97 | 823.62 | 11.39 | 3,456.40 |

### Daily Trends

The Daily Trends worksheet summarizes daily:

- Number of orders
- Total sales
- Quantity

It also contains a Daily Total Sales Trend line chart.

The highest daily sales recorded were 9,290.49 on August 20, 2023, while the lowest were 24.48 on July 12, 2024.

## Key Findings

- Quantity has a mean of 2.95 and median of 3.00.
- UnitPrice has a mean of 356.41 and median of 364.21.
- ItemsInCart has a mean of 5.49 and median of 5.00.
- TotalPrice has a mean of 1,053.97, compared with a median of 823.62.
- The TotalPrice mean is noticeably higher than its median, indicating that higher values are pulling the average upward.
- Daily sales vary considerably, with the highest daily sales of 9,290.49 and the lowest of 24.48 identified in the analysis.

## Outlier Analysis

Outliers were identified using the Interquartile Range (IQR) method. The workbook explicitly notes that flagged values are not automatically errors.

| Variable | Outliers |
|---|---:|
| Quantity | 0 |
| UnitPrice | 0 |
| ItemsInCart | 0 |
| TotalPrice | 8 |

A total of 8 IQR-based outliers were identified, all in TotalPrice.

The Outlier Details worksheet lists the affected orders and their corresponding dates, quantities, unit prices, items in cart, and total prices. The identified TotalPrice values range from 3,334.00 to 3,456.40.

The workbook's analysis treats these as higher TotalPrice observations rather than automatically classifying them as errors. Their presence is consistent with the observation that higher values are pulling the TotalPrice mean above its median.

## Tools & Technologies

- Microsoft Excel

## Workbook Structure

- README — Project purpose, analysis areas, and deliverables.
- Dataset — Original dataset containing 1,200 orders and 14 columns.
- Basic Statistics — Descriptive statistics for the main numerical variables.
- Daily Trends — Daily orders, sales, and quantity, including the Daily Total Sales Trend chart.
- Outlier Summary — IQR calculations, bounds, and outlier counts for the numerical variables.
- Outlier Details — Details of the 8 identified TotalPrice outliers.
- Key Insights — Consolidated statistical observations, daily sales highs/lows, and outlier findings.

## Project Outcome

The completed EDA provides a structured summary of the numerical characteristics of the order data, daily sales activity, and potential outliers. The main findings show variation in daily sales and a higher-than-median average TotalPrice, with 8 IQR-based outliers identified exclusively in TotalPrice. The workbook documents these observations without automatically treating the flagged values as errors.
