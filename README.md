# dbscan-optics-clustering

# DBSCAN and OPTICS Clustering on Bank and Iris Datasets

This project demonstrates the application of DBSCAN and OPTICS clustering algorithms on two different datasets: the **Bank dataset** and the **Iris dataset**. The goal is to explore density-based clustering techniques and evaluate their performance on real-world and benchmark datasets.

---

## Features of the Datasets

### Bank Dataset:
- **ID**: Unique identifier for each customer.
- **Balance**: Number of miles eligible for award travel.
- **Qual_mile**: Miles qualifying for top-tier status.
- **Credit Card Miles**:
  - `cc1_miles`: Miles earned with frequent flyer credit card.
  - `cc2_miles`: Miles earned with rewards credit card.
  - `cc3_miles`: Miles earned with small business credit card.
- **Bonus Miles**: Miles earned from non-flight bonus transactions.
- **Bonus Transactions**: Non-flight bonus transactions in the past 12 months.
- **Flight Miles (12 months)**: Miles flown in the past year.
- **Flight Transactions (12 months)**: Number of flights in the past year.
- **Days Since Enrolled**: Days since the customer joined the frequent flyer program.
- **Award**: Indicator of whether the customer received an award flight.

### Iris Dataset:
- **Sepal Length**: Length of the sepal (cm).
- **Sepal Width**: Width of the sepal (cm).
- **Petal Length**: Length of the petal (cm).
- **Petal Width**: Width of the petal (cm).
- **Species**: The species of the iris flower.

---

## Key Steps in the Project

### 1. Data Preprocessing:
- Imported necessary libraries like `sklearn`, `pandas`, and `numpy`.
- Scaled the features using `StandardScaler` and `MinMaxScaler` to ensure compatibility with clustering algorithms.

### 2. Exploratory Data Analysis (EDA):
- Visualized data distributions and outliers using:
  - Heatmaps
  - Box plots
  - Scatter plots
- Analyzed relationships between features.

### 3. Clustering Algorithms:
#### **DBSCAN**:
- Explored a range of parameters (`eps` and `min_samples`) to identify clusters.
- Evaluated cluster quality using Silhouette Score.
- Applied DBSCAN to both datasets and compared results.

#### **OPTICS**:
- Used the OPTICS algorithm to detect clusters and hierarchical relationships.
- Generated reachability plots to analyze cluster structures.

### 4. Visualization:
- Plotted clustering results using t-SNE and PCA for better interpretability.
- Highlighted clusters using scatter plots and reachability graphs.

---

## Results and Insights

### Bank Dataset:
- DBSCAN and OPTICS successfully identified customer groups based on credit card usage, bonus transactions, and flight activity.
- Clustering insights reveal potential target segments for loyalty programs.

### Iris Dataset:
- Both algorithms accurately distinguished between iris species, showcasing their effectiveness in well-separated clusters.

---

## Conclusion
- **DBSCAN** is effective for datasets with noise and arbitrary-shaped clusters.
- **OPTICS** excels in visualizing hierarchical cluster relationships.
- Both methods provide valuable insights for customer segmentation and species classification.
