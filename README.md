# ***Understanding Mental Health Inequality on a Global Scale***

### **Introduction**
Mental health plays a vital role in overall well-being of a person, and yet, mental healthcare remains one of the most unequally distributed health services across the world. While some countries have robust mental health policies and specialist availability, others face gaps in care, funding, and infrastructure. These disparities are often shaped by deeper structural and socioeconomic differences.

This project aims to analyze global mental health indicators using real-world, country-level datasets. We apply different machine learning techniques/models to uncover hidden patterns and build predictive models that help us better understand access to mental healthcare across nations.

## Project Contents

- `code/mental_health_code.ipynb` – Final codebook  
- `code/basic_cleaning.ipynb` – Basic cleaning codebook 
- `data/raw_data/access_to_care/` – Global mental health care data on healthcare services, financing, policies, and workforce, etc.  
- `data/raw_data/disorders/` – Prevalence and death rates for mental disorders (anxiety, depression, etc.)  
- `data/raw_data/substance_use/` – Alcohol and drug use disorder data by age, sex, and country  
- `Mental_Health_Report.pdf` – Final blog/report (to be added)  
- `README.md` – Project overview  
- `images/` – Contains all the plot images from the codebook
- `blog_post` – Blog post for the project 

---

## Visual Analysis
- PCA Projection Plot:
   To visualize countries in 2D space using the first two principal components.
  
- Scree Plot:
   To show how much variance is explained by each principal component (PCA).

- KMeans Cluster Scatterplot:
  To visualize the clusters formed by KMeans on PCA-reduced data.
  
- Elbow Plot (K-Means)
   To determine the optimal number of clusters by analyzing Within-Cluster Sum of Squares    (WCSS).

- Dendrograms (Hierarchical Clustering):
  To show nested clustering relationships using Ward linkage.

- Decision Tree Plot
  To visually explain how the decision tree splits data based on disorder rates to predict legislation access.

- Confusion Matrix
  To visually evaluate model performance by showing correct vs incorrect predictions.
---

## Methods

- Unsupervised learning
    - PCA
    - Hierarchial Clustering
    - K-Means Clustering
      
- Supervised Learning
    - Decision Tree
    - Random Forest
    - SVM
    - Regression
    - Logistic Regression

---

## Summary

The project successfully demonstrated that machine learning is a powerful tool for both uncovering complex global patterns and disparities in mental health burdens and for accurately predicting the existence of critical access-related infrastructure. This provides valuable insights for understanding the global mental health landscape and potentially informing policy and resource allocation.

---

Submitted by: *Mahek Patel*
