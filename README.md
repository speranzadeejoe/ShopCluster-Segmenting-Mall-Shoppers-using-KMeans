
## 🛍️ **ShopCluster: Segmenting Mall Shoppers using KMeans**

A machine learning project for segmenting shopping mall customers based on their **annual income**, **spending score**, and optionally **gender**, using **KMeans clustering**. The goal is to help mall management better understand customer groups for targeted marketing.

---

### 📊 Objective

- Group customers into meaningful segments using **unsupervised learning**.
- Compare clustering performance **with and without gender** as a feature.
- Evaluate cluster quality using the **Silhouette Score**.
- Visualize the clusters for business insights.

---

### 🧰 Tech Stack

- **Language:** Python  
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

### 📂 Dataset

The dataset includes:
- `Gender` (Male/Female)
- `Annual Income (k$)`
- `Spending Score (1-100)`

---

### 🚀 Workflow

#### 1. **Preprocessing**
- Select features for clustering.
- Scale the data using `StandardScaler`.

#### 2. **Clustering Without Gender**
- Use `Annual Income` and `Spending Score` only.
- Apply **KMeans** with `n_clusters=5`.
- Evaluate using **Silhouette Score** → `0.55` (Good cluster separation).

#### 3. **Clustering With Gender**
- Encode `Gender` numerically (Male: 1, Female: 0).
- Include `Gender`, `Annual Income`, and `Spending Score`.
- Apply **KMeans** with `n_clusters=5`.
- Silhouette Score → `0.40` (Lower than without gender).

#### 4. **Visualization**
- 2D scatter plots of clusters with color-coded segments.

---

### 📈 Results

| Model               | Features Used                              | Silhouette Score |
|--------------------|---------------------------------------------|------------------|
| Without Gender      | `Annual Income`, `Spending Score`          | **0.55**         |
| With Gender         | `Gender`, `Annual Income`, `Spending Score`| 0.40             |

**Conclusion:**  
Excluding gender resulted in better-defined clusters. This suggests that gender may not significantly influence customer grouping in this dataset.

---

### 📌 Key Learnings

- How to implement **KMeans** in Python.
- The importance of **feature selection** in unsupervised learning.
- How to evaluate clustering with **Silhouette Score**.
- Effective **data visualization** for business storytelling.

---
