# 🛒 Intelligent Retail Demand Forecasting & Inventory Optimization

An end-to-end **Data Science and Machine Learning project** that combines multiple retail datasets to analyze sales, customer behavior, promotions, demand patterns, and inventory performance. The project transforms raw data into actionable business insights and inventory optimization recommendations using **Python, Pandas, NumPy, Scikit-learn, and statistical techniques**.

## 📊 Datasets Used

The project integrates four complementary retail datasets:

* 🏪 **Walmart Store Sales** — sales analysis and demand forecasting
* 🛍️ **Rossmann Store Sales** — promotion and store performance analysis
* 📦 **Supply Chain Inventory Dataset** — inventory and supply-chain analysis
* 🛒 **Instacart Market Basket Dataset** — customer and product purchasing behavior

Rather than directly merging unrelated datasets, each dataset is processed independently and their results are standardized into a **Unified KPI Table** for overall business analysis.

## 🔄 Project Workflow

```text
Raw Retail Data
      ↓
Data Cleaning & Preprocessing
      ↓
Exploratory Data Analysis (EDA)
      ↓
Feature Engineering
      ↓
Demand Forecasting
      ↓
Promotion & Customer Analytics
      ↓
Inventory Optimization
      ↓
Risk Analysis
      ↓
Unified KPI Table
      ↓
Business Insights
```

## 🔍 Key Analysis Performed

### 🧹 Data Cleaning & Preprocessing

* Missing-value handling
* Duplicate removal
* Data type conversion
* Outlier analysis
* Date/time preprocessing
* Categorical data processing
* Dataset validation

### 📈 Exploratory Data Analysis

* Sales trends
* Store performance
* Product performance
* Customer purchasing behavior
* Promotion impact
* Demand variability
* Inventory patterns

### 🤖 Demand Forecasting

* Time-based feature engineering
* Lag features
* Rolling averages
* Seasonal features
* Historical demand analysis
* Random Forest Regression
* Time-based train/test split
* Model evaluation using **MAE, RMSE, MAPE, and R²**

### 🏷️ Promotion Analytics

* Promotional vs non-promotional sales
* Promotion lift percentage
* Customer response to promotions
* Store-level performance
* Sales trends during promotional periods

### 🛒 Customer & Product Analytics

* Product popularity
* Customer purchasing behavior
* Reorder rate
* Basket size
* Frequently reordered products
* Department-level performance
* Product-level analysis

### 📦 Inventory Optimization

* Demand variability analysis
* Safety Stock calculation
* Reorder Point (ROP)
* Economic Order Quantity (EOQ)
* Recommended Order Quantity
* Stockout risk identification
* Overstock risk identification
* Inventory decision analysis

## 📊 Unified KPI Framework

A standardized KPI table is created across all datasets to provide a consistent business view.

| Dataset         | KPI Examples                                              |
| --------------- | --------------------------------------------------------- |
| 🏪 Walmart      | Total Sales, Forecast Demand, Forecast Error, Store Count |
| 🛍️ Rossmann    | Total Sales, Customers, Promotion Lift, Store Count       |
| 📦 Supply Chain | Inventory Metrics, Demand, Stockout Risk, Overstock Risk  |
| 🛒 Instacart    | Customers, Orders, Products, Reorder Rate, Basket Size    |

The final KPI structure follows:

```text
Dataset
KPI Category
KPI
Value
Unit
```

This makes the outputs consistent and easy to analyze across different business domains.

## 📁 Major Outputs

```text
📂 data/processed/
│
├── walmart_forecast.csv
├── walmart_feature_importance.csv
├── rossmann_promotion_analysis.csv
├── rossmann_daily_insights.csv
├── supply_chain_analysis.csv
├── inventory_optimization.csv
├── instacart_product_behavior.csv
├── instacart_department_analysis.csv
├── instacart_basket_analysis.csv
└── unified_kpi_table.csv
```

## 🧠 Technologies Used

**Python** • **Pandas** • **NumPy** • **Scikit-learn** • **Matplotlib** • **Seaborn** • **Joblib**

### 🎯 Skills Demonstrated

**Data Analysis** • **EDA** • **Data Cleaning** • **Data Preprocessing** • **Feature Engineering** • **Demand Forecasting** • **Machine Learning** • **Regression** • **Model Evaluation** • **Inventory Optimization** • **Supply Chain Analytics** • **Customer Analytics** • **KPI Development** • **Business Insights**

## 💡 Business Objective

The primary objective is to help retail businesses **understand demand, identify important sales and customer patterns, optimize inventory levels, reduce stockout and overstock risks, and make data-driven replenishment decisions** using historical retail data.

> 🚀 **Outcome:** A complete retail analytics and machine-learning solution that connects **demand forecasting, promotion analysis, customer behavior, inventory optimization, and unified KPI analysis** into one practical data science project.
