# 🛒 E-Commerce Sales & Customer Performance Dashboard Analysis

> A comprehensive, end-to-end multi-table e-commerce analysis project evaluating regional sales, product category profitability, customer segmentation, and payment gateway distributions using Advanced Excel, Power Query, and Power BI.

---

## 📌 Project Executive Summary
This capstone project transforms raw multi-source transactional logs into a structured relational star-schema model. By integrating **Customer, Product, Store, and Sales** dimensions, the analysis delivers a centralized Executive Dashboard that highlights high-performing revenue drivers, payment channel preferences, and customer loyalty tiers.

---

## 🏗️ Relational Data Architecture & Star Schema
The underlying data model links four core normalized tables:

```text
[Customer_Dim] (1) ------< (N) [Sales_Fact] (N) >------ (1) [Product_Dim]
                                     ^
                                     | (1:N)
                              [Store_Dim]
---

## 🧹 Data Cleaning & ETL Pipeline (Power Query & M)
Prior to modeling and dashboarding, raw operational data underwent rigorous preprocessing:
* **Null & Missing Value Handling**: Imputed missing categorical attributes with default tags and standardized demographic records.
* **Data Type Enforcement**: Converted date fields, monetary values, and integer counts to precise data types.
* **Calculated Metrics**: Built custom calculated columns for **Gross Revenue** (Quantity $\times$ Unit Price) and **Net Profitability**.

---

## 📊 Dashboard Visual Breakdown & Key Performance Indicators (KPIs)

The centralized **Executive Dashboard** (`Executive Dashboard` worksheet) features interactive slicers and dark-themed visual panels:

| Metric / Visual Panel | Key Insights & Findings |
| :--- | :--- |
| **Total Gross Revenue** | Generated robust multi-channel sales totaling **$1,196,026.36** across fiscal periods. |
| **Total Units Sold** | Achieved a cumulative sales volume of **2,666 units** across all retail categories. |
| **Revenue by Product Category** | **Electronics** and **Clothing** lead total transaction value, driven by high unit pricing and steady seasonal demand. |
| **Revenue by Payment Method** | **Credit Cards** and **Digital Wallets/PayPal** dominate checkout preferences, minimizing cash-on-delivery lag. |
| **Top 10 Stores by Revenue** | Flagship urban storefronts outperform suburban outlets by **1.8x** in average basket size. |
| **Revenue Breakdown by Gender & Loyalty** | Platinum and Gold tier members across both male and female demographics contribute the highest lifetime value. |

---

## 🛠️ Tools & Technologies Used
* **Microsoft Excel**: Advanced formulas (`XLOOKUP`, `SUMIFS`), Pivot Tables, Conditional Formatting, and Executive Dashboard Layouts.
* **Power Query**: Automated data ingestion, relational merging, and structural transformations.
* **Power BI Desktop**: Data modeling, cross-filter cardinality setup, and interactive visual rendering.
* **GitHub**: Repository hosting, version control, and documentation.
