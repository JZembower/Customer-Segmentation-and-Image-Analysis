# Customer Segmentation and Behavior Prediction

This project analyzes customer data to segment customers and predict their future purchase behavior.

## Project Overview

The project aims to provide insights into customer behavior through segmentation and to build a predictive model for future purchases.

## Author

Jonah Zembower

## Date

May 7, 2024

## Data

The project utilizes the `customer_data.csv` dataset, which includes customer demographics (age, gender, annual income), purchase history (total purchases, average purchase value, most purchased product category), engagement metrics (website visits, marketing emails opened, support call hours), and churn status. The dataset also includes a `Future_Purchase` target variable.

### Data Preprocessing

Data preprocessing involved handling missing values (none found), one-hot encoding categorical features, and standardizing numerical features. No features were removed due to correlation.

## Methodology

### Customer Segmentation

Both K-means and Hierarchical Clustering were used for customer segmentation. K-means with 3 clusters was preferred. Three customer personas were identified:

* **"Engaged General Shoppers"**: Moderate engagement, higher support calls.
* **"Affluent, Casual Shoppers"**: Higher incomes, highest average purchase values, moderate engagement, minimal support time.
* **"Economical, Active Browsers"**: Lowest average purchase values and total purchases, active website visits with less purchase commitment.

### Predictive Modeling

Various machine learning models were developed to predict future purchases, including Logistic Regression, Neural Networks, Decision Trees, SVM, Random Forest, and Gradient Boosting.

* **Random Forest** showed promising results.
* An optimal threshold of **0.3** for Random Forest was found, yielding an F1 score of **0.795** and improving recall.

### PCA Analysis

Principal Component Analysis (PCA) revealed that approximately **73.6% of the variance** is explained by the first 6 components, with variance tapering off after the 8th component.

## Technologies Used

The project was developed in Python, leveraging libraries such as:

* **pandas**: Data manipulation.
* **matplotlib** and **seaborn**: Data visualization.
* **numpy**: Numerical operations.
* **scikit-learn**: Data preprocessing, clustering, and predictive modeling.
* **tensorflow.keras**: Neural network development.

## Files in the Repository

* `customer_data.csv`: The dataset.
* `Final_Project.ipynb`: Jupyter Notebook with all analysis and code.
* `Final Project.pptx`: Project presentation slides.
* `README.md`: This README file.
