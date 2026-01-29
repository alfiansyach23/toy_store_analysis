🧸 Toy Store E-Commerce Data Analysis

Author: Alfian Syach

📌 Project Overview

This project is an end-to-end data analysis case study based on the Toy Store E-Commerce (Maven Fuzzy Factory) dataset.
The goal of this project is to analyze website activity, marketing performance, and transaction data to better understand business performance and support data-driven decision making.

The project covers the full data workflow, from raw data extraction to transformation, loading, and analysis preparation.

🎯 Business Objectives

The main objectives of this project are:

Analyze website traffic and sales trends

Evaluate conversion performance

Assess marketing channel effectiveness

Analyze revenue-related metrics

📂 Dataset Description

The dataset is sourced from Maven Analytics – Toy Store E-Commerce Database, representing an end-to-end e-commerce business flow, starting from website sessions to orders and refunds.

Main Tables

website_sessions

website_pageviews

orders

order_items

order_item_refunds

products

🔗 Data Source:
https://mavenanalytics.io/data-playground/toy-store-e-commerce-database

🔍 Data Understanding & Data Quality
Data Quality Checks

No duplicate records found

All columns were checked for consistency and unique values

Missing values were identified only in specific marketing-related columns

Missing Values

Missing values were found in the website_sessions table, specifically in:

utm_source

utm_campaign

utm_content

http_referrer

Handling Strategy

Missing values in UTM-related columns were filled with "unknown"

This approach helps:

Prevent aggregation bias

Maintain consistency in marketing channel analysis

Improve interpretability for non-technical stakeholders

The implementation was done using Python, while the logic is also explained using SQL-style CASE WHEN for clarity.

🔄 End-to-End ETL Process
1. Extract

Data extracted from the Toy Store E-Commerce database

Stored as raw CSV files

2. Transform

Data cleaning and preprocessing

Missing value handling

Performed using Python

3. Load

Cleaned and structured data loaded into MySQL

Used for further analysis and querying

🛠 Tools & Technologies

Python (Data cleaning & transformation)

SQL / MySQL (Data storage & querying)

Pandas & NumPy

Data Visualization (trend and performance charts)
