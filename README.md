
# eCommerce Transactions Dataset Analysis

## Overview

This project involves analyzing an eCommerce transactions dataset to derive business insights, build a Lookalike Model, and perform customer segmentation using clustering techniques. The dataset consists of three files:

- `Customers.csv`
- `Products.csv`
- `Transactions.csv`

The analysis is performed using Python in Google Colab, with libraries such as Pandas, Matplotlib, and Scikit-learn.

## Prerequisites

Before running the project, ensure the following dependencies are installed:

- Python 3.x
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab (or any preferred IDE)

## Dataset Description

1. **Customers.csv**:
   - `CustomerID`: Unique identifier for each customer.
   - `CustomerName`: Name of the customer.
   - `Region`: Continent where the customer resides.
   - `SignupDate`: Date when the customer signed up.

2. **Products.csv**:
   - `ProductID`: Unique identifier for each product.
   - `ProductName`: Name of the product.
   - `Category`: Product category.
   - `Price`: Product price in USD.

3. **Transactions.csv**:
   - `TransactionID`: Unique identifier for each transaction.
   - `CustomerID`: ID of the customer who made the transaction.
   - `ProductID`: ID of the product sold.
   - `TransactionDate`: Date of the transaction.
   - `Quantity`: Quantity of the product purchased.
   - `TotalValue`: Total value of the transaction.
   - `Price`: Price of the product sold.

## Analysis Performed

### Task 1: Exploratory Data Analysis (EDA) and Business Insights

- Performed exploratory data analysis (EDA) to understand the dataset and uncover hidden patterns:
  - Checked for missing data, data types, and summary statistics.
  - Visualized customer distribution, product categories, and transaction patterns over time.

- **Business Insights**:
  1. Identified the most popular product categories based on total sales.
  2. Analyzed the average spending patterns of customers across different regions.
  3. Found trends in customer behavior regarding the timing of transactions (seasonality).
  4. Identified high-value customers based on total purchase value.
  5. Determined the most frequently purchased products and their demand.

### Task 2: Lookalike Model

- Built a Lookalike Model to recommend similar customers based on their profile and transaction history:
  - Used customer demographic features (e.g., Region, SignupDate) and transaction patterns (e.g., TotalValue, Frequency).
  - Applied cosine similarity or KNN to find similar customers.

- Generated a `Lookalike.csv` file containing the top 3 lookalike customers for the first 20 customers, considering factors like region and spending behavior.

### Task 3: Customer Segmentation / Clustering

- Performed customer segmentation using clustering techniques such as K-means:
  - Extracted features such as total purchase value, frequency of purchases, and recency of transactions.
  - Applied K-means clustering to group customers into distinct segments.

- **Evaluation**:
  - Evaluated the clustering results using the Davies-Bouldin Index (DB Index), ensuring the clusters are well-separated.

- **Visualization**:
  - Visualized the clusters using scatter plots, showing the distribution of customers based on their segmentation.

## Results and Conclusion

- **Business Insights**:
  - Observed that customers from certain regions tend to spend more, suggesting targeted marketing strategies for those regions.
  - High-value customers were concentrated in a few product categories, highlighting the importance of these products in driving revenue.

- **Lookalike Model**:
  - The model successfully identified similar customers based on purchase history, offering valuable insights for targeted marketing campaigns.

- **Customer Segmentation**:
  - The clustering results revealed distinct customer segments based on their purchasing behavior, such as high-spending and frequent buyers. These insights can be used for personalized marketing efforts and improving customer retention strategies.


