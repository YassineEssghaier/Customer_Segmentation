# Customer Segmentation with Kmeans Clustering 



Project Overview
This project aims to segment customers based on their credit card usage data using unsupervised learning techniques. The goal is to understand customer behavior and group customers with similar profiles for targeted marketing or personalized services.

Dataset
The dataset used is the Credit Card General dataset from Statso (link to dataset: https://statso.io/customer-segmentation-case-study/#google_vignette).

The dataset includes various features such as:

BALANCE: The current balance on the customer's credit card.

CREDIT_LIMIT: The maximum amount the customer can borrow.

PAYMENTS: Payments made by the customer.

MINIMUM_PAYMENTS: Minimum required payments.

And many other features related to customer behavior.

Steps Taken
Data Cleaning:

Removed the CUST_ID column, which is not useful for analysis.

Handled missing values by filling NaN entries with the median of each column.

Data Scaling:

Used StandardScaler to scale the numerical features to have zero mean and unit variance, making them suitable for KMeans clustering.

Clustering:

Applied the KMeans algorithm to segment customers into clusters.

Used the Elbow Method to determine the optimal number of clusters (k=4).

Cluster Visualization:

Reduced data dimensions using PCA and t-SNE to visualize the clusters in 2D.

Modeling:

Trained a Random Forest classifier to predict customer clusters.

Evaluated the model using classification metrics such as precision, recall, and F1-score.

Cluster Evaluation:

Calculated the Silhouette Score and Davies-Bouldin Index to assess the quality of the clusters.

Dependencies
pandas

numpy

scikit-learn

matplotlib

seaborn

To install the necessary libraries, run:

pip install pandas numpy scikit-learn matplotlib seaborn

Results:
The Elbow Method indicated that k=4 was the optimal number of clusters.

The clusters were visualized using PCA and t-SNE, revealing distinct groupings based on customer behavior.

A Random Forest classifier achieved good performance in predicting the clusters.

Conclusion:
This project demonstrates the use of unsupervised learning techniques (KMeans clustering) to segment customers based on their credit card usage behavior. The resulting clusters can be used for targeted marketing, fraud detection, or offering personalized services.
