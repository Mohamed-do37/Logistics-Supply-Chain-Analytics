# 🚚 Logistics Supply Chain Analysis & Delay Prediction

A comprehensive Data Mining and Machine Learning project aimed at diagnosing and predicting supply chain delays. This repository contains a full end-to-end pipeline: from raw data cleaning and SQL database normalization to Exploratory Data Analysis (EDA) and Machine Learning deployment.

## 📌 Project Overview
The logistics network was experiencing a critical **68.1% delay rate**. Using a dataset of 6,880 shipments (March 2019 – Dec 2020), this project identifies the root causes of these bottlenecks and builds a predictive model to flag high-risk shipments before departure. 

## 🏗️ Technical Architecture

### 1. Database & SQL Engineering
* **Normalized Schema:** Designed a highly relational SQL database to replace flat-file chaos.
* **Advanced Queries:** Implemented 10 analytical SQL queries (Views, Joins, Aggregations) and CRUD operations for robust data governance.

### 2. Data Quality & EDA
* **6-Stage Cleaning Pipeline:** Handled severe missing data, duplicate tracking events, and invalid telemetry (e.g., impossible coordinates).
* **Feature Engineering:** Extracted 6 new predictive features, including tracking telemetry types and routing distances.
* **Deep Analytics:** Conducted comprehensive Univariate, Bivariate, and Multivariate analyses to uncover systemic operational flaws.

### 3. Machine Learning (Delay Prediction)
* **Model:** Built a **Random Forest** classifier to predict whether a shipment will be delayed.
* **Risk Thresholding:** Configured the model to flag shipments crossing a `>0.7` delay probability threshold for proactive intervention.

## 📊 Key Strategic Insights
1. **The Telemetry Gap:** GPS infrastructure is a massive predictor of success. Shipments tracked via specific providers (e.g., VAMOSYS) have drastically lower delay rates.
2. **The Client Bottleneck:** A single client (Larsen & Toubro) accounts for **57% of total network volume** but suffers from an **80% delay rate**, indicating severe loading-bay bottlenecks rather than transit issues.
3. **Proactive Intervention:** Deploying the predictive ML model to live operations allows dispatchers to shift from reactive firefighting to proactive resource allocation.

## 🚀 Technologies & Tools Used
* **Database:** Microsoft SQL Server (T-SQL, Schema Design, Views).
* **Data Processing & ML:** Python (Pandas, NumPy, Scikit-Learn).
* **Analytics & Visualization:** Jupyter Notebooks, Matplotlib, Seaborn.
* **Framework:** TQV (Technical, Quality, Value) Standard.
