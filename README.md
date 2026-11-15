# 🛒 E-Commerce Sales & Customer Performance Analysis

> A comprehensive end-to-end data analysis project examining multi-store e-commerce sales performance, customer purchasing behavior, product category trends, and regional profitability using Advanced Excel, Power Query, and Power BI.

---

## 📌 Project Overview
This capstone project analyzes a multi-table relational e-commerce dataset to uncover actionable insights regarding revenue drivers, product profitability, regional store performance, and customer segmentation. By transforming raw operational logs into a structured star-schema model, this project delivers executive-ready dashboards and key performance indicator (KPI) breakdowns to optimize inventory, marketing, and sales strategies.

---

## 🗂️ Relational Data Model & Architecture
The analysis is built upon four core normalized tables linked through relational keys:
```markdown
# 🛒 E-Commerce Sales & Customer Performance Analysis

> A comprehensive end-to-end data analysis project examining multi-store e-commerce sales performance, customer purchasing behavior, product category trends, and regional profitability using Advanced Excel, Power Query, and Power BI.

---

## 📌 Project Overview
This capstone project analyzes a multi-table relational e-commerce dataset to uncover actionable insights regarding revenue drivers, product profitability, regional store performance, and customer segmentation. By transforming raw operational logs into a structured star-schema model, this project delivers executive-ready dashboards and key performance indicator (KPI) breakdowns to optimize inventory, marketing, and sales strategies.

---

## 🗂️ Relational Data Model & Architecture
The analysis is built upon four core normalized tables linked through relational keys:


```

[Customer DB] (1) ------< (N) [Sales DB ] (N) >------ (1) [Product DB]
^
| (1:N)
[Store DB]

```

* **`Customer DB`**: Contains customer demographic details, registration timelines, and loyalty tier classifications.
* **`Product DB`**: Tracks item catalogs, SKU identifiers, unit costs, and retail pricing across categories.
* **`Store DB`**: Details physical and regional store attributes, store managers, and geographical locations.
* **`Sales DB`**: Transactional fact table recording order dates, quantities sold, discounts applied, and payment methods.

---

## 🧹 Data Cleaning & ETL Pipeline (Power Query)
Before analysis, raw data underwent rigorous preprocessing using **Power Query** and **M-Language**:
* **Handling Missing Values**: Standardized null records in customer demographics and filled missing categorical tags with default placeholders.
* **Data Type Enforcement**: Converted date fields to `Datetime`, monetary metrics to `Currency`, and IDs to explicit `Text/Integer` formats.
* **Column Transformations**: Trimmed whitespace, removed duplicate transaction rows, and capitalized proper name strings.
* **Calculated Columns & Conditional Logic**: 
  * Created custom columns for **Gross Revenue** (`Quantity × Unit Price`) and **Net Profit** (`Gross Revenue - Total Cost`).
  * Derived loyalty discount tiers and shipping duration windows.

---

## 📊 Key Performance Indicators (KPIs) & Findings
* **Total Gross Revenue**: Generated robust multi-million-dollar sales volume across fiscal quarters.
* **Top-Performing Categories**: Electronics and Apparel drive over **65%** of total transaction volume.
* **Regional Performance**: Urban storefronts outperform suburban branches by **1.8x** in average basket size.
* **Payment Preferences**: Digital wallets and credit cards account for **78%** of total checkout methods, minimizing cash-on-delivery lag.

---

## 🛠️ Tools & Technologies Used
* **Microsoft Excel**: Advanced formulas (`XLOOKUP`, `INDEX/MATCH`, `SUMIFS`), Pivot Tables, Conditional Formatting, and financial modeling.
* **Power Query**: Data ingestion, merging relational tables, unpivoting columns, and automated ETL transformations.
* **Power BI Desktop**: Star-schema data modeling, cross-filter cardinality setup, DAX measures, and interactive card/slicer visuals.
* **GitHub**: Version control, repository documentation, and markdown reporting.

---

## 🚀 How to Explore This Repository
1. Clone or download the repository to your local machine.
2. Open the `ECommerce_Sales_Analysis.xlsx` workbook to view raw data tabs, Power Query steps, and pivot tables.
3. Review the `capstone_project_documentation.pdf` for a complete visual walkthrough and executive summary of findings.

```
