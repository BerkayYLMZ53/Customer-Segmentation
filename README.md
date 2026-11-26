# Credit Card Customer Segmentation with K-Means

An unsupervised learning project that explores patterns in credit-card customer spending behaviour and groups customers with similar characteristics.

## Project objective

The aim is to identify behavioural segments using features such as spending frequency, cash-advance activity, and credit-limit utilization. Such exploratory segments can help analysts formulate questions for further investigation; they should not be treated as definitive customer risk or creditworthiness labels.

## Dataset and preprocessing

The project uses a commonly available Credit Card Dataset. The workflow includes:

- Handling missing values with `SimpleImputer`.
- Standardizing features with `StandardScaler`, since K-Means is distance-based.
- Applying Principal Component Analysis (PCA) to support dimensionality reduction and two-dimensional cluster visualization.

## Methods and technologies

- **Algorithm:** K-Means clustering
- **Cluster evaluation:** Elbow Method and Silhouette Score
- **Dimensionality reduction:** PCA
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## Exploratory findings

The notebook selects four clusters based on the Elbow Method and Silhouette Score analysis and discusses them as broad behavioural profiles:

1. Lower-spending / lower-utilization customers.
2. Higher-spending / higher-frequency customers.
3. Customers with comparatively higher cash-advance activity.
4. Customers with intermediate spending and payment patterns.

These descriptions are exploratory interpretations of the dataset, not validated business segments or individual credit-risk assessments. Cluster meaning depends on feature selection, preprocessing, and the dataset sample.

## Run locally

Clone the repository:

```bash
git clone https://github.com/BerkayYLMZ53/Customer-Segmentation.git
cd Customer-Segmentation
```

Install the dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

Launch Jupyter Notebook and open `K-Means_Odev.ipynb`.

