# Optimizing E-Commerce Logistics and Customer Segmentation Using Machine Learning

## Table of Contents
1. [Project Overview](#project-overview)
2. [Problem Statement](#problem-statement)
3. [How AI Helps](#how-ai-helps)
4. [Objective](#objective)
5. [Dataset Overview](#dataset-overview)
6. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
7. [Feature Engineering](#feature-engineering)
8. [Model Development](#model-development)
9. [Results and Insights](#results-and-insights)
10. [Conclusion](#conclusion)
11. [How to Run the Project](#how-to-run-the-project)
12. [Contact](#contact)

## **Project Overview**
In the fast-paced e-commerce industry, timely deliveries and effective customer engagement are crucial. However, frequent delivery delays and inefficient customer segmentation can lead to poor customer satisfaction and financial losses. This project leverages machine learning techniques to:
- Predict delivery delays and cancellations.
- Segment customers based on their purchasing behavior.

We approached this problem with a structured data-driven workflow that includes **data preprocessing, exploratory data analysis (EDA), feature engineering, model selection, hyperparameter tuning, and model evaluation**. The goal is to derive meaningful insights that can help optimize delivery logistics and customer targeting.

## **Problem Statement**
E-commerce businesses face challenges such as:
- Late deliveries due to unpredictable supply chain inefficiencies.
- Increased cancellations and customer dissatisfaction.
- Generic marketing strategies failing to address diverse customer needs.
- Lack of personalized engagement leading to reduced customer retention.

By addressing these issues with **classification models for delivery delays** and **clustering techniques for customer segmentation**, we aim to improve both logistics and marketing strategies.

## **How AI Helps**
Machine learning can:
- Predict delivery outcomes using historical order data, enabling proactive logistics management.
- Cluster customers based on purchasing patterns, allowing businesses to offer targeted promotions and loyalty programs.
- Identify factors affecting delivery efficiency, allowing for better operational adjustments.

## **Objective**
1. **Classification Task:** Predict delivery delays and cancellations to enhance logistics planning and customer satisfaction.
2. **Clustering Task:** Segment customers to tailor marketing campaigns and optimize business strategies.

## **Dataset Overview**
The dataset consists of e-commerce transactions, including features such as:
- **Order Details:** Order ID, date, delivery status, shipping type.
- **Customer Information:** Region, city, segment.
- **Transaction Details:** Sales amount, discount, profit, order quantity.
- **Shipping Data:** Scheduled vs. real shipping time.

### **Why This Approach?**
- We first conducted an **exploratory data analysis (EDA)** to understand key patterns and relationships within the dataset.
- We used **feature engineering** to extract meaningful features and remove redundant ones.
- To ensure robust model training, we applied **scaling, encoding, and data balancing** where necessary.
- For classification, we chose **tree-based models** due to their ability to handle imbalanced data and categorical variables effectively.
- For clustering, we experimented with **K-Means and DBSCAN** to identify distinct customer segments.

## **Exploratory Data Analysis (EDA)**
### **Key Insights:**
- **54.8% of orders are delayed**, highlighting a logistics issue.
- **Outliers detected** in sales, discounts, and profits, requiring scaling.
- **First-class shipping has the highest delays**, making it unreliable.
- **Late deliveries impact customer retention**, with order numbers declining over time.

## **Feature Engineering**
- **Removed irrelevant columns** like customer names and order IDs to avoid data leakage.
- **Converted date columns** into numeric features (year, month) for better temporal analysis.
- **Checked multicollinearity** and dropped redundant variables to improve model efficiency.
- **Performed chi-square tests** to retain only significant categorical features, ensuring meaningful predictive relationships.

## **Model Development**
### **Classification (Delivery Delay Prediction):**
- **Models Used:** Decision Trees, Random Forest, Gradient Boosting.
- **Why These Models?**
  - Decision Trees provide an interpretable baseline.
  - Random Forest improves performance through ensemble learning.
  - Gradient Boosting optimizes learning with iterative corrections.
- **Best Model:** Random Forest with an accuracy of **XX%**.
- **Hyperparameter tuning** improved precision and recall, reducing false positives and negatives.

### **Clustering (Customer Segmentation):**
- **Techniques Used:** K-Means, DBSCAN.
- **Why These Methods?**
  - K-Means is efficient and effective in identifying distinct customer groups.
  - DBSCAN handles noise and irregular distribution patterns better.
- **Optimal Clusters:** X clusters found, representing distinct customer behaviors.

## **Results and Insights**
- **Random Forest outperformed other classifiers**, achieving the best balance between precision and recall.
- **Key factors influencing delivery delays** include shipping type, region, and order quantity.
- **Customer segmentation helped differentiate high-value vs. discount-driven buyers.**

## **Conclusion**
This project demonstrates how AI can optimize e-commerce operations by improving logistics and personalizing customer engagement. Future enhancements include:
- Integrating real-time order tracking data.
- Experimenting with deep learning for better predictions.
- Refining customer segmentation using additional behavioral attributes.

---
Clone this repository:
   ```bash
   git clone https://github.com/MNitin-Reddy/Optimizing-E-Commerce-Logistics-and-Customer-Segmentation-Using-Machine-Learning.git
   ```
Run the notebook:
   ```bash
   jupyter notebook AIML_240151939.ipynb
   ```
