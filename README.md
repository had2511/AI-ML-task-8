# AI-ML-task-8
# 🛍️ Mall Customer Segmentation using K-Means

This project performs customer segmentation using **K-Means Clustering** on the **Mall Customer Segmentation Dataset**. The goal is to group customers based on their spending behavior and income to better understand market patterns.

---

## 📁 Dataset

- **Source:** [Kaggle - Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Features:**
  - `CustomerID`
  - `Gender`
  - `Age`
  - `Annual Income (k$)`
  - `Spending Score (1-100)`

---

## ✅ Project Workflow

### 1. Load and Preprocess Data
- Upload the CSV to Google Colab.
- Drop `CustomerID` and encode `Gender`.
- Normalize features using `StandardScaler`.

### 2. PCA (Optional)
- Reduce dimensions using **PCA** to 2D for visualization.

### 3. Elbow Method
- Determine optimal number of clusters (K) by plotting **inertia**.

### 4. K-Means Clustering
- Apply `KMeans` clustering with optimal K.
- Assign cluster labels to each customer.

### 5. Visualize Clusters
- Visualize clusters using:
  - PCA components
  - Original features like `Annual Income` vs `Spending Score`

### 6. Evaluate Clustering
- Calculate **Silhouette Score** to assess cluster quality.

---

## 📊 Technologies Used

- Python
- Google Colab
- pandas
- matplotlib
- seaborn
- scikit-learn

---

## 📈 Key Results

- Optimal number of clusters: **5**
- **Silhouette Score:** ~0.55 (indicates good clustering structure)
- PCA and scatter plots show distinct customer groups based on spending behavior and income.

---

## 📌 Insights

- Customers can be grouped into segments such as:
  - High income, low spending
  - Low income, high spending
  - Average income and spending
- These insights can help businesses target marketing strategies better.

---

## ▶️ How to Run

1. Open the notebook in Google Colab.
2. Upload the dataset (`Mall_Customers.csv`) using:

   ```python
   from google.colab import files
   files.upload()
