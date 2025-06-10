# MSCS 634 - Lab Assignment 3: Clustering with K-Means and K-Medoids on Wine Dataset

## 🧑‍🎓 Student Details  
**Name:** Chandra Kiran Billingi  
**Course:** MSCS 634 – Machine Learning  
**Lab Title:** Clustering Using K-Means and K-Medoids  
**Dataset:** Wine Dataset from scikit-learn

---

## 🔍 Purpose of the Lab  
In this lab, I explored unsupervised learning techniques by applying both K-Means and K-Medoids clustering algorithms to the Wine dataset. The primary goal was to understand how different clustering algorithms group data points based on similarity and how well these clusters align with the actual wine classes. Evaluation metrics like **Silhouette Score** and **Adjusted Rand Index (ARI)** were used to assess cluster quality and alignment with ground truth labels.

---

## 📊 Key Insights from Clustering Results

### K-Means Clustering:
- We have Produced distinct and well-separated clusters based on the feature space.
- We have also calculated Silhouette Score which was relatively high which indicates well-defined clustering structure.
- ARI score showed good agreement with actual class labels.
- This model Performs best when data is spherical and evenly distributed around the centroid.

### K-Medoids Clustering:
- We have also produced interpretable clusters but slightly lower performance compared to K-Means.
- More robust to outliers due to the use of actual data points (medoids) as centers.
- Required custom implementation using `scipy` and `numpy` due to compatibility issues with `sklearn-extra`.

### Comparison:
- **K-Means** had better clustering scores and clearer separation visually.
- **K-Medoids** handled noisy/outlier-like samples better but required more manual implementation and tuning.
- **K-Means** is preferable for speed and simplicity, while **K-Medoids** is suitable when data has irregular distributions or is sensitive to outliers.

---

## ⚠️ Challenges Faced
- Implementing **K-Medoids** without `sklearn-extra` was challenging due to environment and version conflicts with the installed libraries.
- Required debugging and manual coding using **NumPy** and **SciPy** to perform medoid selection and distance calculations.
- Visualizing clusters accurately and marking centroids/medoids needed careful plotting and interpretation.

---
