# ***Understanding Mental Health Inequality on a Global Scale***

### **Overview**
This project explores the global burden of mental health disorders and investigates how various countries provide access to mental health policy, services, and legislation. Using a combination of unsupervised and supervised machine learning techniques, we identify hidden patterns in the data and develop predictive models to understand the factors associated with mental health access indicators.

The analysis is presented as part of a comprehensive communication deliverable in the form of a well-documented Jupyter notebook hosted on GitHub. The deliverable includes clearly explained code, visualizations, and interpretations designed for both technical and general audiences.

---

### **Objective:**
1. Identify underlying structure in global mental health data using dimensionality reduction and clustering.
2. Understand the relationships between mental health burden and policy access across countries.
3. Build supervised models to predict whether a country has mental health legislation based on disorder rates.
4. Provide actionable insights through visual analytics and interpretability-focused methods.

---

## Datasets Used

- **DALY Data**: Disability-Adjusted Life Years (DALYs) for multiple mental health disorders (2019–2021).
- **Policy Access Data**: Country-wise availability of mental health policy, services, and legislation (including years of implementation).
- **GDP Data**: Country GDP to explore correlations with access and burden.
- All datasets were sourced from publicly available global health and economic data repositories.

---

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

## Methods and Techniques

### Data Preprocessing
- Cleaned and merged multiple datasets using consistent country codes.
- Converted year-wise access indicators into binary flags.
- Handled missing values using `SimpleImputer` for supervised models.
- Aggregated and reshaped disorder data into modeling format.

### Unsupervised Learning
- **Principal Component Analysis (PCA)**: Reduced dimensionality and visualized underlying variance structure.
- **KMeans Clustering**: Grouped countries based on PCA-transformed data to identify similar profiles.
- **Hierarchical Clustering (Ward linkage)**: Explored alternative groupings and compared them with KMeans results.

### Supervised Learning
- Target Variable: Binary indicator of whether a country has **mental health legislation**.
- Features: Average DALY rates for 6 major disorders.
- Models Used:
  - Logistic Regression
  - Random Forest
  - Support Vector Machine (SVM)
  - Decision Tree
- Evaluated with confusion matrix, precision, recall, f1-score, and accuracy.

---

## Visual Analytics

- **Scree Plot**: Visualized explained variance from PCA.
- **PCA Projection Scatterplots**: Colored by continent and cluster.
- **Elbow Plot**: Helped choose optimal `k` for KMeans.
- **Dendrogram**: Visualized hierarchical clustering structure.
- **Model Decision Tree Plot**: Interpreted rules used for prediction.
- **Confusion Matrices**: Evaluated model performance.

---

## Key Findings

- PCA revealed strong separation between countries based on access and burden.
- KMeans with `k=4` provided interpretable groupings aligned with regional and economic similarities.
- Supervised models performed well, with Random Forest and SVM achieving the highest accuracy and F1-scores.
- Eating Disorders and Depression were highly influential in predicting policy presence.

---


## Summary

The project successfully demonstrated that machine learning is a powerful tool for both uncovering complex global patterns and disparities in mental health burdens and for accurately predicting the existence of critical access-related infrastructure. This provides valuable insights for understanding the global mental health landscape and potentially informing policy and resource allocation.

---

Submitted by: *Mahek Patel*
