# 🧠 Understanding K-Means Clustering: How the Number of Clusters (K) Impacts Machine Learning Performance

**👨‍💻 Author:** K Pradeep Raj (24145399)

---

## 📖 Project Overview

Customer segmentation is a fundamental business analytics technique that enables organizations to understand customer behavior, improve marketing strategies, and enhance customer retention.

This project explores the application of the **K-Means Clustering Algorithm** to segment mall customers based on their annual income and spending behavior.

A key challenge in K-Means clustering is determining the optimal number of clusters (**K**). Selecting too few clusters may oversimplify customer groups, while selecting too many may create unnecessary complexity and reduce interpretability.

---

## 🎯 Project Objectives

The primary objectives of this project are to:

* ✅ Understand the principles of unsupervised machine learning
* ✅ Implement K-Means clustering for customer segmentation
* ✅ Investigate the impact of varying the number of clusters (K)
* ✅ Apply feature scaling using StandardScaler
* ✅ Evaluate clustering performance
* ✅ Interpret customer segments from a business perspective
* ✅ Explore ethical considerations in customer analytics
* ✅ Demonstrate accessibility-aware data visualization practices

---

## 📂 Dataset Information

### 🗄️ Dataset

**Mall Customer Segmentation Dataset**

### 🌐 Source

Kaggle

### 📋 Dataset Description

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| CustomerID             | Unique customer identifier            |
| Gender                 | Customer gender                       |
| Age                    | Customer age                          |
| Annual Income (k$)     | Annual income in thousands of dollars |
| Spending Score (1-100) | Mall-assigned spending score          |

### 🎯 Features Used for Clustering

* 💰 Annual Income (k$)
* 🛍️ Spending Score (1–100)

---

## ⚙️ Methodology

### 🔍 1. Exploratory Data Analysis (EDA)

Initial analysis was conducted to:

* 📈 Understand feature distributions
* 🔎 Identify patterns and trends
* 🧩 Detect potential clustering structures
* 📊 Visualize customer behavior

---

### 🧹 2. Data Preprocessing

Since K-Means uses Euclidean distance, feature scaling is essential.

✔️ Standardization was performed using StandardScaler.

---

### 🤖 3. K-Means Clustering

K-Means partitions observations into K clusters by minimizing within-cluster variance.

#### Workflow

1. 🎯 Initialize centroids
2. 📍 Assign data points to nearest centroid
3. 🔄 Update centroid positions
4. ✅ Repeat until convergence

---

### 🎛️ 4. Hyperparameter Tuning

The primary hyperparameter explored was:

* 🔢 Number of Clusters (K)

Different values of K were tested to evaluate:

* 📏 Cluster compactness
* 📐 Cluster separation
* 🧠 Interpretability
* 💼 Business usefulness

---

### 📊 5. Cluster Evaluation

#### 📉 Elbow Method

Measures:

* Within-Cluster Sum of Squares (WCSS)

Used to identify the optimal K value.

---

#### 📈 Silhouette Analysis

Measures:

* Cohesion within clusters
* Separation between clusters

Score Interpretation:

| Score | Meaning                 |
| ----- | ----------------------- |
| 🔴 -1 | Poor clustering         |
| 🟡 0  | Overlapping clusters    |
| 🟢 +1 | Well-separated clusters |

---

## 🏆 Results and Findings

Based on quantitative evaluation and business interpretability, the optimal number of clusters was:

# ⭐ K = 5

The model identified five distinct customer segments.

### 👑 Cluster 1: High Income – High Spending

**VIP Customers**

Characteristics:

* 💰 High purchasing power
* 🛒 Frequent spending
* ⭐ High customer value

Business Strategy:

* 🎁 Loyalty rewards
* 💎 Premium memberships
* 🎯 Exclusive offers

---

### 📈 Cluster 2: High Income – Low Spending

**Potential Customers**

Characteristics:

* 💵 Strong financial capacity
* 📉 Lower engagement levels

Business Strategy:

* 🎯 Personalized promotions
* 📢 Targeted marketing
* 📦 Upselling campaigns

---

### 👥 Cluster 3: Average Customers

Characteristics:

* ⚖️ Moderate income
* ⚖️ Moderate spending

Business Strategy:

* 🤝 Retention programs
* 🎉 Seasonal offers

---

### 🛍️ Cluster 4: Low Income – High Spending

Characteristics:

* 💸 Budget-conscious shoppers
* 🛒 Active purchasing behavior

Business Strategy:

* 🏷️ Discount campaigns
* 🎁 Reward programs

---

### 🌱 Cluster 5: Low Income – Low Spending

Characteristics:

* 📉 Limited purchasing activity

Business Strategy:

* 📣 Awareness campaigns
* 💡 Cost-effective engagement

---

## 🚀 Advanced Enhancements

This project extends beyond basic clustering by incorporating:

### 📊 Statistical Evaluation

* ✅ Elbow Method
* ✅ Silhouette Analysis

### 🔧 Hyperparameter Investigation

* ✅ Comparison of multiple K values
* ✅ Cluster stability assessment

### 💼 Business Interpretation

* ✅ Customer personas
* ✅ Marketing recommendations

### ♿ Accessibility-Focused Visualization

* ✅ Colorblind-friendly design
* ✅ Grayscale compatibility
* ✅ High-contrast layouts

---

## ♿ Accessibility Considerations

### 🎨 Colorblind-Friendly Visualizations

* Distinct marker shapes
* Direct centroid labeling
* Reduced reliance on color

### 🔍 High-Contrast Design

* Larger font sizes
* Dashed gridlines
* Clear legends and labels

### 🖨️ Grayscale Compatibility

All visualizations remain interpretable when printed in black and white.

---

## ⚖️ Ethical Considerations

Potential risks include:

* 🚨 Reinforcing socioeconomic biases
* 🚨 Unequal treatment of customer groups
* 🚨 Lack of transparency in automated decision-making

Mitigation strategies:

* 👨‍⚖️ Human oversight
* 🔒 Privacy protection
* 📜 Regulatory compliance

---

## 📁 Repository Structure

```text
K-Means-Clustering/

├── 📂 Outputs/
│   ├── 📊 Comparison of different K values.png
│   ├── 📈 Dataset classification.png
│   ├── 📉 Elbow Method.png
│   ├── 🎯 K-Means Customer Segmentation.png
│   ├── 📋 Silhouette Analysis.png
│   └── ⚙️ Hyperparameter Tuning.png
│
├── 📄 KMeans_report.pdf
├── 📓 K_Means_Clustering_(1).ipynb
├── 🗃️ Mall_Customers.csv
├── 📜 requirements.txt
├── ⚖️ LICENSE
└── 📘 README.md
```

## 🛠️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/K-Means-Clustering.git
```

### 2️⃣ Navigate to Project Folder

```bash
cd K-Means-Clustering
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Launch Jupyter Notebook

```bash
jupyter notebook
```

---

## 📦 Dependencies

* 🐍 Python 3.x
* 🔢 NumPy
* 🐼 Pandas
* 📊 Matplotlib
* 🤖 Scikit-Learn
* 📓 Jupyter Notebook

---

## 🎓 Key Learning Outcomes

Through this project, readers will learn:

* 🧠 Fundamentals of K-Means clustering
* ⚙️ Feature scaling and preprocessing
* 📊 Cluster evaluation techniques
* 🎛️ Hyperparameter tuning
* 💼 Business-oriented interpretation
* ⚖️ Ethical implications of customer analytics
* ♿ Accessible data visualization design

---

## 🔮 Future Work

Potential extensions include:

* 📉 PCA-based dimensionality reduction
* 🌳 Hierarchical clustering
* 🔍 DBSCAN comparison
* 🎲 Gaussian Mixture Models (GMM)
* 🌐 Interactive Streamlit dashboard
* 🤖 Automated recommendation systems
* 📡 Real-time customer segmentation

---

## 📚 References

MacQueen, J. (1967). Some Methods for Classification and Analysis of Multivariate Observations.

Lloyd, S. (1982). Least Squares Quantization in PCM.

Arthur, D., & Vassilvitskii, S. (2007). k-means++: The Advantages of Careful Seeding.

Bishop, C. M. (2006). Pattern Recognition and Machine Learning.

Hastie, T., Tibshirani, R., & Friedman, J. (2009). The Elements of Statistical Learning.

---

## ⚖️ License

Licensed under the **MIT License**.
The project is created for academic purpose, you may reuse the code with proper attribution

---

## 🙏 Acknowledgements

Special thanks to:

* 🏢 Kaggle for providing the dataset
* 🤖 Scikit-Learn for machine learning tools
* 🐍 Python open-source community

⭐ If you found this project useful, consider starring the repository and sharing your feedback!

