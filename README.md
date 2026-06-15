# K-Means Customer Segmentation: Understanding the Impact of K on Clustering Quality

**Author:** K Pradeep Raj (24145399)
---

## Project Overview

This project demonstrates the application of K-Means clustering to a real-world customer segmentation problem using the Mall Customer Segmentation dataset. The tutorial focuses on understanding how the choice of the number of clusters (K) affects clustering quality, interpretability, and business insights.

K-Means is one of the most widely used unsupervised machine learning algorithms. It partitions observations into clusters by minimizing the distance between data points and their assigned cluster centroids. Since the number of clusters must be specified beforehand, selecting an appropriate value of K is critical for obtaining meaningful results.

The project investigates this challenge using both the Elbow Method and Silhouette Analysis and provides visual and business interpretations of the resulting customer segments.

---

## Learning Objectives

The objectives of this project are to:

* Understand the principles of K-Means clustering.
* Investigate the impact of the number of clusters (K).
* Apply feature scaling using StandardScaler.
* Evaluate clustering quality using the Elbow Method.
* Evaluate clustering quality using Silhouette Analysis.
* Interpret clusters from a business perspective.
* Consider ethical implications of customer segmentation.
* Demonstrate accessibility-aware data visualization practices.

---

## Dataset

### Dataset Name

Mall Customer Segmentation Dataset

### Source

Kaggle

### Features

| Feature                | Description                           |
| ---------------------- | ------------------------------------- |
| CustomerID             | Unique customer identifier            |
| Gender                 | Gender of customer                    |
| Age                    | Customer age                          |
| Annual Income (k$)     | Annual income in thousands of dollars |
| Spending Score (1-100) | Mall-assigned spending score          |

### Features Used for Clustering

This project uses:

* Annual Income (k$)
* Spending Score (1-100)

These features provide a meaningful representation of customer purchasing power and spending behaviour while allowing clear visualization of cluster formation.

---

## Methodology

### Data Exploration

The dataset was initially explored using descriptive statistics and scatter plots to understand customer distributions and identify potential clustering patterns.

### Feature Scaling

StandardScaler was applied before clustering because K-Means relies on Euclidean distance calculations. Feature scaling ensures that both variables contribute equally to cluster formation.

### K-Means Clustering

K-Means clustering was applied to identify groups of customers with similar characteristics.

The objective function minimized by K-Means is:

J = Σ(i=1→K) Σ(x∈Ci) ||x−μi||²

where μi represents the centroid of cluster i.

### Cluster Evaluation

Two methods were used to determine the optimal number of clusters:

#### Elbow Method

Measures Within-Cluster Sum of Squares (WCSS) across different K values.

#### Silhouette Analysis

Measures how well-separated clusters are from one another.

### Final Model

The final model was trained using K = 5 based on evaluation results and business interpretability.

---

## Results

The clustering process identified distinct customer groups including:

* High Income, High Spending (VIP Customers)
* High Income, Low Spending (Potential Customers)
* Average Customers
* Low Income, High Spending Customers
* Low Income, Low Spending Customers

These customer segments can support targeted marketing strategies and customer retention efforts.

---

## Accessibility Considerations

Accessibility was incorporated throughout the project.

The following measures were implemented:

### Colorblind-Friendly Visualizations

* Distinct marker shapes were used for different clusters.
* Centroids were labelled directly on plots.
* Figures remain interpretable without colour.

### High Contrast Design

* Dashed gridlines improve readability.
* Larger font sizes support users with visual impairments.
* Clear axis labels and legends were included.

### Grayscale Compatibility

Visualizations remain understandable when printed in black and white.

These design choices ensure the tutorial can be accessed by a broader audience and align with inclusive data visualization practices.

---

## Ethical Considerations

Customer segmentation can provide valuable business insights but may also introduce ethical concerns.

Potential risks include:

* Reinforcing socioeconomic biases.
* Unequal treatment of customer groups.
* Lack of transparency in automated decision-making.

To address these concerns, clustering results should support human decision-making rather than replace it, and customer data should be handled in accordance with relevant privacy regulations.

---

## Dependencies

* Python 3.x
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

---

## References

MacQueen, J. (1967). Some Methods for Classification and Analysis of Multivariate Observations.

Lloyd, S. (1982). Least Squares Quantization in PCM.

Arthur, D., & Vassilvitskii, S. (2007). k-means++: The Advantages of Careful Seeding.

Bishop, C. M. (2006). Pattern Recognition and Machine Learning.

Hastie, T., Tibshirani, R., & Friedman, J. (2009). The Elements of Statistical Learning.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.
This is to hereby declare that this project can be used by anyone for learning and implementing into thier work and requesting to give suitable comments and  reviews regrading any add-ons or changes to be done in the code. 
