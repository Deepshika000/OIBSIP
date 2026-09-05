# Customer Segmentation via K-Means Clustering

# Project Overview
This module applies machine learning algorithms to group customers into distinct behavioral personas based on their purchasing habits. 
Using normalized RFM (Recency, Frequency, Monetary) metrics, the pipeline identifies key customer segments to drive targeted marketing strategies.

# Machine Learning Pipeline
Feature Selection: Selected key behavioral columns: `Days Since Last Purchase` (Recency), `Items Purchased` (Frequency), and `Total Spend` (Monetary).
Feature Standardization: Scaled features to a mean of 0 and variance of 1 using `StandardScaler` to prevent feature magnitude bias.
Optimal Cluster Selection: Evaluated Within-Cluster Sum of Squares (Inertia) across multiple $K$ values using the **Elbow Method** to select the optimal number of groups.
Segmentation & Profiling: Applied $K$-Means clustering to categorize customers into high-value VIPs, occasional spenders, and at-risk segments.

# Visualizations & Deliverables
Elbow Method Plot: Identified the bend in inertia for optimal cluster selection.
2D Scatter Plots: Visualized cluster boundaries across multiple feature combinations (e.g., Spend vs. Frequency).
Cluster Distribution Bar Chart: Displayed customer count breakdowns per segment.

# Tech Stack
Language: Python
Machine Learning: Scikit-Learn (`KMeans`, `StandardScaler`)
Data & Visualization: Pandas, Matplotlib, Seaborn
