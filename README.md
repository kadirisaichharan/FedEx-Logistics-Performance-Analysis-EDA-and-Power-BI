# FedEx-Logistics-Performance-Analysis-EDA-and-Power-BI

FedEx Logistics Performance Analysis (EDA)
📌 Project Overview
FedEx operates a high-velocity global supply chain. This project analyzes a comprehensive shipment history dataset to evaluate Service Performance, Cost Efficiency, and Operational Reliability. By transforming raw delivery records into actionable KPIs, the analysis identifies bottlenecks in the logistics network and provides data-driven strategies for optimization.

📊 Business Objectives
Identify Operational Inefficiencies: Detect delays and high-cost routes within the global network.

KPI Engineering: Develop metrics for Lead Time, On-Time Delivery (OTD), and Freight Cost per KG.

Strategic Optimization: Provide recommendations to lower operational costs and improve customer satisfaction.

🛠️ Tech Stack
Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn

Environment: Google Colab / Jupyter Notebook

📈 Key Features & Data Wrangling
Date Standardization: Converted inconsistent strings into datetime objects for time-series analysis.

Numerical Cleaning: Cleaned currency and weight strings using Regex to enable mathematical computations.

Feature Engineering: * lead_time: (Delivered Date - PO Sent Date).

on_time: Boolean flag for deliveries meeting the schedule.

freight_per_kg: Normalized cost metric for efficiency comparison.

Imputation: Handled missing values in Shipment Mode and Insurance using statistical medians to maintain distribution integrity.

🔍 Visual Insights
The analysis includes several critical visualizations to understand the logistics flow:

Lead Time Distribution: Visualizing the "Logistics Pulse" to identify systemic bottlenecks.

Cost vs. Mode: Boxplots comparing delivery speeds across Air, Truck, and Ocean modes.

Correlation Heatmap: Uncovering the relationship between shipment weight, value, and freight costs.

💡 Business Recommendations
Route Optimization: Transition high-cost, non-urgent Air shipments to Ground/Ocean modes to reduce freight_per_kg.

Vendor Accountability: Implement a Vendor Scorecard based on the 10% lowest-performing delivery routes.

Seasonality Management: Adjust capacity during identified "Peak Months" where On-Time rates traditionally dip.

📂 Repository Structure
Plaintext
├── SCMS_Delivery_History_Dataset.csv  # Raw Dataset
├── FedEx_Logistics_Analysis.ipynb     # Main Analysis Notebook
├── README.md                          # Project Documentation
└── requirements.txt                   # Python Dependencies

