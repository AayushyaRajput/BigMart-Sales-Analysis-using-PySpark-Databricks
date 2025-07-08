# BigMart-Sales-Analysis-using-PySpark & Databricks
A complete data analysis project using PySpark on Databricks to explore and visualize BigMart sales data. It includes data cleaning, feature engineering, and interactive visualizations created with Databricks' built-in charting tools.

## 📊 Objective

To explore, clean, and analyze the BigMart retail dataset using **PySpark** and visualize trends using **Databricks’ built-in charting tools**. This project focuses on deriving meaningful business insights through structured EDA and feature engineering.

## 🧰 Tools & Technologies

- **Apache Spark (PySpark)** — For distributed data analysis
- **Databricks Notebook** — For cloud-based computation and visualization
- **Spark SQL & PySpark DataFrame API** — For querying and transformations
- **Databricks Visualizations** — Bar charts, pie charts, line graphs (UI-based)

## 🧼 Step 1: Data Cleaning

- ✅ Missing values filled:
  - `Item_Weight`: Replaced with mean per item
  - `Outlet_Size`: Filled using the mode per location
- ✅ Cleaned `Item_Fat_Content` (e.g., standardized `LF`, `low fat`)
- ✅ Added new column: `Years_Since_Establishment` = 2025 - `Outlet_Establishment_Year`

---

## 🏗️ Step 2: Feature Engineering

| Feature | Description |
|--------|-------------|
| `Years_Since_Establishment` | Store age since establishment |
| `MRP_Range` | Categorized item price into bins (Low/Med/High/Very High) |
| `Revenue_per_Weight` | Sales per unit weight |

---

## 🔍 Step 3: Exploratory Data Analysis (EDA)

Used **PySpark + groupBy + Databricks charts** for:

- 📊 Total sales by `Outlet_Type`
- 📈 Sales trend by `MRP_Range`
- 🧈 Distribution of `Item_Fat_Content`
- 📦 Store age vs average sales
- 🛍️ Revenue insights per item category
