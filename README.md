# 🛒 SmartCart: Customer Segmentation & Behavioral Analytics

An end-to-end unsupervised machine learning pipeline designed to segment e-commerce and retail shoppers based on purchasing behaviors, transaction patterns, and cart attributes. Using exploratory data analysis, outlier detection, Principal Component Analysis (PCA), and clustering algorithms, this project extracts actionable business intelligence for targeted marketing and customer retention.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Domain](https://img.shields.io/badge/Domain-Unsupervised%20Learning%20%26%20Analytics-green)
![Clustering](https://img.shields.io/badge/Clustering-K--Means%20%2F%20PCA-orange)

---

## 📌 Executive Summary

Understanding customer purchasing dynamics is vital for retail businesses seeking to personalize offers, optimize inventory, and boost Customer Lifetime Value (CLV). The **SmartCart System** processes complex transactional datasets, standardizes high-dimensional behavioral features, reduces feature dimensionality using PCA, and segments shoppers into distinct behavioral personas using optimal clustering metrics.

---

## 🛠️ Analytics & Unsupervised ML Workflow

### 1. Data Preprocessing & Quality Assurance
- **Data Cleaning & Normalization:** Handled missing values, removed duplicate entries, and parsed transactional features.
- **Feature Scaling:** Standardized continuous behavioral features using `StandardScaler` to eliminate scale bias during distance-based calculations.

### 2. Feature Engineering
- **Behavioral Attributes:** Formulated aggregate metrics capturing shopping frequency, basket size, and spending indicators.
- **Cart Interaction Features:** Engineered normalized ratios to reflect user engagement and purchase velocity.

### 3. Outlier Detection & Correlation Analysis
- **Outlier Identification:** Detected anomalous purchasing patterns using IQR and distance methods to prevent cluster centroid distortion.
- **Multicollinearity Heatmap:** Generated Seaborn correlation matrices to identify feature redundancies and optimize input matrices.

### 4. Dimensionality Reduction (PCA)
- **Principal Component Analysis:** Transformed correlated features into orthogonal principal components, preserving cumulative variance while reducing computational noise.
- **2D/3D Feature Visualization:** Visualized customer clusters across principal component axes for clear interpretability.

### 5. Clustering & Persona Insights
- **Optimal K Evaluation:** Evaluated cluster quality across multiple parameters using the **Elbow Method** and **Silhouette Scores**.
- **Clustering Execution:** Trained K-Means / Hierarchical Clustering to partition customers into distinct groups.
- **Business Persona Insights:** Identified actionable segments such as High-Value Shoppers, Occasional Buyers, and Price-Sensitive Accounts.

---

## 📁 Repository Structure

```text
smartcart-customer-segmentation/
│
├── main.py                # Primary unsupervised ML pipeline (Preprocessing, PCA, Clustering, Insights)
├── requirements.txt       # Project dependencies
├── .gitignore             # Standard Git ignore file
└── README.md              # Project documentation
