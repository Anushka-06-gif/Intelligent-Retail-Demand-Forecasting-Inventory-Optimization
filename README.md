# 🛒 Intelligent Retail Demand Forecasting & Inventory Optimization

An end-to-end **Retail Analytics, Demand Forecasting & Inventory Optimization** project that combines multiple retail and supply-chain datasets to transform raw business data into actionable insights. 📊🚀

The project integrates **Walmart, Rossmann, Supply Chain, and Instacart datasets** to analyze sales trends, customer behavior, promotions, demand patterns, and inventory risks while developing a unified **KPI framework and Power BI-ready business intelligence layer**.

---

## 🎯 Project Objectives

* 📈 Forecast retail demand using Machine Learning
* 🧹 Perform data cleaning and preprocessing
* 🔍 Conduct Exploratory Data Analysis (EDA)
* 📊 Analyze sales and demand trends
* 🏷️ Measure promotion impact and sales lift
* 👥 Analyze customer purchasing behavior
* 🛍️ Identify popular and frequently reordered products
* 📦 Analyze inventory levels and demand variability
* ⚠️ Identify stockout and overstock risks
* 🔄 Calculate Reorder Point and Safety Stock
* 📦 Calculate Economic Order Quantity (EOQ)
* 🎯 Generate recommended order quantities
* 📊 Create unified business KPIs across datasets
* 📈 Build an interactive Power BI dashboard

---

## 📂 Datasets Used

### 🏬 1. Walmart Store Sales Dataset

Used for **sales analysis and demand forecasting**.

Key analysis:

* 💰 Weekly sales analysis
* 🏪 Store-level performance
* 📅 Time-series analysis
* 🌡️ Temperature and economic factor analysis
* 🎯 Holiday impact
* 📈 Demand forecasting
* 🔄 Lag features
* 📊 Rolling statistics
* 🤖 Machine Learning prediction

### 🏪 2. Rossmann Store Sales Dataset

Used for **retail promotion and store performance analytics**.

Key analysis:

* 💰 Sales performance
* 👥 Customer analysis
* 🏪 Store performance
* 🏷️ Promotion vs. non-promotion sales
* 📈 Promotion lift %
* 📅 Daily and seasonal trends
* 📊 Average sales and customer behavior

### 📦 3. High-Dimensional Supply Chain Inventory Dataset

Used as the **core inventory optimization dataset**.

Key analysis:

* 📦 Inventory analysis
* 📈 Demand variability
* ⏱️ Lead-time analysis
* 🛡️ Safety Stock
* 🔄 Reorder Point (ROP)
* 📦 Economic Order Quantity (EOQ)
* ⚠️ Stockout Risk
* 📦 Overstock Risk
* 🎯 Recommended Order Quantity
* 📊 Inventory performance KPIs

### 🛒 4. Instacart Market Basket Dataset

Used for **customer and product behavior analytics**.

Key analysis:

* 👥 Customer purchasing behavior
* 🛍️ Product popularity
* 🔁 Reorder rate
* 🧺 Basket size analysis
* 🏷️ Department performance
* ⭐ Frequently reordered products
* 📊 Product-level analysis
* 👥 Customer-level analysis

---

## 🔄 Project Workflow

```text
📂 Raw Datasets
      ↓
🧹 Data Cleaning & Preprocessing
      ↓
🔍 Exploratory Data Analysis
      ↓
📊 Feature Engineering
      ↓
📈 Demand Forecasting
      ↓
📦 Inventory Analytics
      ↓
🛡️ Safety Stock Calculation
      ↓
🔄 Reorder Point Calculation
      ↓
📦 EOQ Calculation
      ↓
⚠️ Stockout / Overstock Risk
      ↓
🎯 Recommended Order Quantity
      ↓
📊 Unified KPI Table
      ↓
📈 Power BI Dashboard
```

---

## 🤖 Demand Forecasting

The Walmart dataset is used to build a Machine Learning-based demand forecasting model.

### Feature Engineering

* 📅 Year
* 📅 Month
* 📅 Quarter
* 📅 Week
* 📅 Day of Week
* 🔄 Lag features
* 📊 Rolling mean
* 📉 Rolling standard deviation
* 🌐 Cyclical time features
* 🎉 Holiday indicators
* 🌡️ Temperature
* ⛽ Fuel Price
* 💹 CPI
* 📊 Unemployment

### Machine Learning Model

🌲 **Random Forest Regressor**

Model evaluation includes:

* 📏 MAE — Mean Absolute Error
* 📐 RMSE — Root Mean Squared Error
* 📊 MAPE — Mean Absolute Percentage Error
* 🎯 R² Score

---

## 📦 Inventory Optimization

The project converts demand forecasts into practical inventory decisions.

### 🛡️ Safety Stock

```text
Safety Stock =
Z × Demand Standard Deviation × √Lead Time
```

### 🔄 Reorder Point

```text
ROP =
Average Demand × Lead Time + Safety Stock
```

### 📦 Economic Order Quantity

```text
EOQ = √(2DS / H)
```

Where:

* D = Annual Demand
* S = Ordering Cost
* H = Holding Cost

### ⚠️ Risk Classification

Inventory is classified into:

* 🔴 HIGH Stockout Risk
* 🟡 MEDIUM Stockout Risk
* 🟢 LOW Stockout Risk

and:

* 🔴 HIGH Overstock Risk
* 🟡 MEDIUM Overstock Risk
* 🟢 LOW Overstock Risk

---

## 📊 Unified KPI Framework

Instead of directly merging unrelated datasets, the project creates a **common business KPI layer**.

### 💰 Sales KPIs

* Total Sales
* Average Sales
* Store Performance
* Sales Trends

### 📈 Forecasting KPIs

* Forecast Demand
* Prediction Error
* MAE
* RMSE
* MAPE
* R²

### 📦 Inventory KPIs

* Current Stock
* Safety Stock
* Reorder Point
* EOQ
* Recommended Order Quantity
* Stockout Risk
* Overstock Risk

### 🏷️ Promotion KPIs

* Promotion Sales
* Non-Promotion Sales
* Promotion Lift %
* Promotion Rate

### 👥 Customer KPIs

* Total Customers
* Total Orders
* Average Basket Size
* Reorder Rate
* Product Popularity

---

## 📊 Power BI Dashboard

The processed datasets and unified KPI table are designed for an interactive **Power BI Business Intelligence dashboard**.

### 📌 Dashboard Sections

**🏠 Executive Overview**

* Total Sales
* Forecast Demand
* Inventory Risk
* Recommended Orders
* Customer Metrics

**📈 Demand Forecasting**

* Actual vs Predicted Demand
* Sales Trends
* Store Performance
* Forecast Error
* Feature Importance

**📦 Inventory Optimization**

* Stockout Risk
* Overstock Risk
* Safety Stock
* Reorder Point
* EOQ
* Recommended Order Quantity

**👥 Customer & Product Analytics**

* Top Products
* Reorder Rate
* Basket Size
* Department Performance
* Customer Behavior

**🏷️ Promotion Analytics**

* Promotion vs Non-Promotion Sales
* Promotion Lift
* Store Promotion Performance

---

## 📁 Project Outputs

The pipeline generates Power BI-ready CSV files such as:

```text
📁 data/processed/
│
├── 📊 walmart_forecast.csv
├── 📊 walmart_feature_importance.csv
├── 🏷️ rossmann_promotion_analysis.csv
├── 📈 rossmann_daily_insights.csv
├── 📦 inventory_optimization.csv
├── ⚠️ stockout_risk.csv
├── 🎯 reorder_recommendations.csv
├── 👥 customer_behavior.csv
├── 🛒 product_behavior.csv
├── 🏷️ department_analysis.csv
├── 🧺 basket_analysis.csv
└── 📊 unified_kpi_table.csv
```

---

## 🛠️ Technologies Used

🐍 **Python**
🐼 **Pandas**
🔢 **NumPy**
🤖 **Scikit-learn**
🌲 **Random Forest**
📊 **Matplotlib**
📈 **Power BI**
📓 **Jupyter / Google Colab**
💾 **CSV / Data Processing**
🔧 **Git & GitHub**

---

## 💡 Business Value

This project demonstrates how multiple retail datasets can be transformed into a practical **data-driven decision-support system**.

It helps answer important business questions such as:

* 📈 How much demand can we expect?
* 🏪 Which stores are performing best?
* 🏷️ How much do promotions increase sales?
* 📦 How much inventory should be maintained?
* ⚠️ Which locations/products are at risk of stockouts?
* 📦 Where is excess inventory accumulating?
* 🔄 When should inventory be reordered?
* 🎯 How much should be ordered?
* 👥 Which products and customers show strong repeat-purchase behavior?

---

## 🚀 Key Skills Demonstrated

**Data Analysis • Exploratory Data Analysis (EDA) • Data Cleaning • Data Preprocessing • Feature Engineering • Time-Series Forecasting • Machine Learning • Predictive Analytics • Inventory Optimization • Demand Forecasting • Safety Stock • Reorder Point • EOQ • Risk Analysis • KPI Development • Business Intelligence • Data Visualization • Power BI Dashboard Development • Customer Analytics • Retail Analytics**

---

## 👩‍💻 Project Outcome

The final solution provides a complete analytical workflow from:

**Raw Data → Data Cleaning → EDA → Feature Engineering → ML Forecasting → Inventory Optimization → Risk Analysis → KPI Development → Power BI Business Intelligence Dashboard** 📊🚀
