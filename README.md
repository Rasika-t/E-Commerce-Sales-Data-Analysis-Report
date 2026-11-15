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
