# Task 2 - Customer Segmentation using K-Means

## Project Overview
This project focuses on customer segmentation using the K-Means clustering algorithm.

The goal is to group customers based on their purchasing behavior so that businesses can create targeted marketing strategies.

## Dataset
The project uses the Online Retail Dataset from the UCI Machine Learning Repository.

Dataset Source:
https://archive.ics.uci.edu/dataset/352/online+retail

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Methodology

### 1. Data Cleaning
- Removed records with missing CustomerID.
- Removed cancelled transactions.
- Removed invalid Quantity and UnitPrice values.
- Created a new TotalAmount column.

### 2. RFM Analysis
Customer behavior was analyzed using three RFM features:

- Recency - Number of days since the customer's last purchase.
- Frequency - Number of unique invoices/purchases made by the customer.
- Monetary - Total amount spent by the customer.

### 3. Data Preprocessing
- Applied log transformation to RFM values.
- Standardized the features using StandardScaler.

### 4. K-Means Clustering
The K-Means algorithm was applied to segment customers.

The Elbow Method was used to evaluate different values of K.

The final model uses 4 customer segments.

## Customer Segments

| Cluster | Customer Segment | Count |
|--------|------------------|------:|
| 0 | Recent / Promising Customers | 837 |
| 1 | High-Value Loyal Customers | 716 |
| 2 | Regular Customers | 1,173 |
| 3 | At-Risk / Inactive Customers | 1,612 |

## Marketing Insights

### High-Value Loyal Customers
- Provide VIP rewards.
- Offer early access to new products.
- Provide premium bundles and loyalty benefits.

### Recent / Promising Customers
- Encourage repeat purchases.
- Use cross-selling and personalized recommendations.

### Regular Customers
- Offer personalized discounts.
- Promote loyalty points.
- Recommend relevant products.

### At-Risk / Inactive Customers
- Send win-back campaigns.
- Provide special discounts.
- Use re-engagement emails.

## Project Files

- `Task_2_Customer_Segmentation_KMeans.ipynb` - Jupyter Notebook containing the complete analysis.
- `customer_segmentation_rfm.csv` - Final customer segmentation results.

## Conclusion
K-Means clustering successfully segmented customers based on their purchasing behavior.

These customer segments can help businesses design targeted marketing campaigns, improve customer retention, and increase customer value.
