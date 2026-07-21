# Supply Chain Delivery Performance Analysis & Late Delivery Prediction

> An end-to-end data analytics and machine learning project that analyzes global supply chain delivery performance, identifies operational bottlenecks, quantifies the financial impact of delivery delays, and predicts late deliveries using a Random Forest classifier.

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-purple)

---

# Project Overview

Efficient supply chain management is critical for customer satisfaction and business profitability. Even small delays in delivery can significantly impact customer trust, increase operational costs, and reduce profit margins.

This project performs an end-to-end analysis of a global e-commerce supply chain dataset to:

- Analyze delivery performance
- Measure profitability and financial risk
- Detect operational bottlenecks
- Identify root causes of delayed deliveries
- Discover temporal delivery patterns
- Build a predictive machine learning model to identify orders at risk of being delivered late

The project combines **Business Intelligence**, **Exploratory Data Analysis**, **Statistical Analysis**, and **Machine Learning** into one complete analytics workflow.

---

# Business Problem

A global e-commerce company delivers products across multiple regions using different shipping methods.

Despite having multiple logistics channels, a large proportion of customer orders arrive later than promised, leading to:

- Reduced customer satisfaction
- Loss of profitability
- Poor shipping reliability
- Inefficient operational planning

The objective of this project is to identify **why delays occur**, determine **their business impact**, and develop a predictive model capable of identifying high-risk deliveries before shipment.

---

# Project Objectives

- Perform comprehensive exploratory data analysis
- Clean and preprocess supply chain data
- Calculate business KPIs
- Analyze delivery performance
- Measure profitability
- Detect operational bottlenecks
- Perform regional and temporal analysis
- Build a machine learning model for delay prediction
- Generate actionable business recommendations

---

# Dataset

The project uses the **DataCo Global Supply Chain Dataset**, which contains transactional information about customer orders, products, shipping, logistics, and profitability.

The dataset includes information such as:

- Customer Details
- Product Information
- Department
- Shipping Mode
- Market
- Region
- Country
- Delivery Status
- Scheduled Shipping Time
- Actual Shipping Time
- Order Profit
- Order Date
- Shipping Date
- Payment Method

---

# Technologies Used

### Programming

- Python

### Data Analysis

- Pandas
- NumPy

### Data Visualization

- Matplotlib
- Seaborn

### Machine Learning

- Scikit-learn
- Random Forest Classifier
- SMOTE (Imbalanced Learning)

### Jupyter Notebook

- Interactive data exploration

---

# Project Workflow

## 1. Data Loading

- Import dataset
- Explore dataset dimensions
- Check missing values
- Inspect data types

---

## 2. Data Cleaning

The following preprocessing steps were performed:

- Removed duplicate records
- Removed unnecessary personal information
- Converted date columns into datetime format
- Handled missing values
- Dropped irrelevant columns
- Created derived features
- Feature engineering for analysis

---

## 3. Exploratory Data Analysis (EDA)

Several visualizations were created to understand the dataset.

### Business KPIs

- Total Orders
- Total Profit
- Late Deliveries
- On-Time Deliveries
- Profit at Risk
- Average Profit per Order
- Delay Percentage

---

### Profitability Analysis

Analysis includes:

- Profit Distribution
- Loss-making Orders
- Break-even Orders
- Profit vs Delay Days
- Delay Distribution

---

### Delivery Performance Analysis

Performance comparison across:

- Shipping Modes
- Customer Segments
- Regions
- Departments
- Order Status
- Payment Type

---

### Root Cause Analysis

Detailed investigation of:

- High delay regions
- Shipping bottlenecks
- Payment processing delays
- Department-wise delay rates

---

### Time-Based Analysis

Delivery delays analyzed across:

- Month
- Weekday
- Hour of Day

This helps identify seasonal peaks and operational bottlenecks.

---

# Machine Learning Model

## Problem Type

Binary Classification

Target Variable

```
Late_delivery_risk
```

Where

- 0 → On-Time Delivery
- 1 → Late Delivery

---

## Data Preprocessing

The ML pipeline includes:

- Frequency Encoding
- Train-Test Split
- Feature Scaling (where required)
- SMOTE for balancing classes

---

## Model Used

Random Forest Classifier

Reasons for selection:

- Handles categorical data well
- Robust to noisy data
- Captures nonlinear relationships
- High predictive performance
- Easy feature importance analysis

---

# Model Performance

| Metric | Score |
|---------|------:|
| Accuracy | **74%** |
| Precision | **74%** |
| Recall | **74%** |
| F1 Score | **74%** |

The model provides a strong baseline for identifying deliveries likely to be delayed, enabling proactive operational intervention.

---

# 📌 Key Business Insights

## Delivery Performance

- More than half of all orders were delivered late.
- Late deliveries represent the default operational outcome rather than isolated incidents.

---

## Shipping Modes

Shipping mode has the greatest impact on delivery performance.

- First Class experienced the highest delay rate.
- Second Class also showed significant delays.
- Standard Class performed considerably better.
- Same Day shipping achieved the best performance.

---

## Regional Analysis

Delay rates remained relatively consistent across regions, indicating that the problem is systemic rather than location-specific.

---

## Profitability

Most orders remained profitable.

However,

- Loss-making orders were concentrated among delayed shipments.
- Delayed deliveries place millions of dollars of profit at risk.

---

## Seasonal Trends

Peak delays occurred during:

- August
- September
- December

suggesting demand surges overwhelm fulfillment capacity.

---

## Operational Bottlenecks

Major contributors include:

- Shipping mode selection
- Payment processing delays
- Inventory management
- Fulfillment workflow inefficiencies

---

# Business Recommendations

The analysis recommends:

- Audit premium shipping services
- Optimize shipping mode allocation
- Deploy predictive delay alerts
- Improve payment processing workflows
- Increase logistics capacity during seasonal peaks
- Continuously retrain prediction models
- Improve warehouse operations
- Monitor delivery KPIs in real time

---

# Repository Structure

```
Supply-Chain-Delivery-Analysis/
│
├── Supply Chain Complete Analysis.ipynb
├── Supply_Chain_Performance_Report.pdf
├── README.md
```

---

# 📊 Visualizations Included

The notebook contains professional visualizations such as:

- KPI Dashboard
- Profit Distribution
- Delay Distribution
- Profit vs Delay
- Shipping Mode Analysis
- Region-wise Delay Analysis
- Customer Segment Analysis
- Department Analysis
- Payment Type Analysis
- Monthly Delay Trends
- Weekly Delay Trends
- Hourly Delay Trends
- Confusion Matrix
- Feature Importance

---

# Future Improvements

Possible enhancements include:

- XGBoost and LightGBM models
- Hyperparameter tuning
- Deep learning approaches
- Real-time prediction API
- Interactive Power BI/Tableau dashboard
- Explainable AI using SHAP values
- Integration with live logistics systems

---

# How to Run the Project

### Clone Repository

```bash
git clone https://github.com/yourusername/Supply-Chain-Delivery-Performance.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

If no `requirements.txt` is available, install:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

### Launch Notebook

```bash
jupyter notebook
```

Open:

```
Supply Chain Complete Analysis.ipynb
```

Run all cells sequentially.

---

# 📈 Learning Outcomes

This project demonstrates practical experience in:

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Business Intelligence
- Data Visualization
- KPI Design
- Machine Learning
- Random Forest Classification
- SMOTE
- Business Recommendation Generation
- End-to-End Data Analytics

---



# ⭐ If you found this project useful

Please consider giving this repository a **Star ⭐** to support the project.
