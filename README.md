# 💳 Credit Card Customer Segmentation with K-Means (Unsupervised Learning)

This project is an unsupervised learning study developed to analyze the financial behaviors and spending habits of credit card users, aiming to assist in guiding banking strategies by creating **customer segments (clusters)**.

## 🎯 Project Objective
To identify groups exhibiting similar behaviors by examining financial metrics such as customers' spending frequency, cash advance tendencies, and credit limit utilization; thereby helping to develop personalized marketing and risk management strategies.

## 📊 Dataset, Preprocessing, and Dimensionality Reduction
The **"Credit Card Dataset"**, commonly used in the machine learning community, was utilized in this study. The following preprocessing steps were applied during the data preparation phase:
* **Missing Value Imputation:** Missing values in the dataset were filled using the `SimpleImputer` library to preserve the overall data distribution.
* **Feature Scaling:** Since the K-Means algorithm is distance-based, all variables were standardized using `StandardScaler`.
* **PCA (Principal Component Analysis):** Dimensionality reduction was applied to address multicollinearity issues in the high-dimensional dataset and to visualize the clusters on a 2D plane.

## 🛠️ Technologies and Methods Used
* **Programming Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn
* **Method:** K-Means Clustering & Silhouette Score Analysis

## 📈 Clustering Results and Customer Profiles
Based on the evaluation of the Silhouette Score and the Elbow Method, the number of clusters was set to **4**. The customers were grouped into the following financial behavior segments:
1. 🎯 **Cluster 0 (Passive Customers):** A standard segment characterized by low spending and low credit utilization.
2. 💎 **Cluster 1 (High-Value Customers):** The segment with high spending frequency and volume, representing high profitability for the bank.
3. ⚠️ **Cluster 2 (At-Risk Customers):** Customers with a high tendency to use their credit limits for cash advances and a higher propensity for debt/interest.
4. 📈 **Cluster 3 (Mid-Tier Customers):** A segment with moderate spending and payment balances, representing future potential.

## 🚀 Running the Project Locally
```bash
git clone https://github.com/BerkayYLMZ5353/customer-segmentation-kmeans.git
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook K-Means_Odev.ipynb
```
