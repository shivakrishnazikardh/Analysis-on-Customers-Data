

# 📊 Marketing Campaign Analysis & Customer Segmentation using Machine Learning

## 📝 Overview

This project aims to analyze a marketing campaign dataset and perform customer segmentation using clustering techniques. It includes comprehensive data preprocessing, feature engineering, exploratory data analysis, visualization, and the application of machine learning models for classification and clustering. The final objective is to derive customer insights that can guide marketing strategies.

---

## 📁 Dataset

The dataset used is a CSV file named:

```
marketing_campaign excel.csv
```

It contains detailed customer information including demographics, purchase behavior, and campaign responses.

---

## 🔧 Tools and Libraries Used

| **Tool/Library**       | **Purpose**                                                                 
|------------------------|------------------------------------------------------------------------------
| **Pandas**             | Data manipulation and analysis                                               
| **NumPy**              | Numerical computations                                                       
| **Matplotlib**         | Static data visualization                                                    
| **Seaborn**            | Statistical data visualization                                               
| **Scikit-learn (sklearn)** | Machine learning algorithms, scaling, model selection, metrics              
| **Yellowbrick**        | Model visualization (Elbow & Silhouette for clustering)                     
| **RobustScaler**       | Outlier-resistant feature scaling                                            
| **PCA (Principal Component Analysis)** | Dimensionality reduction                                     
| **KMeans**             | Clustering algorithm                                                         
| **RandomForestClassifier, GradientBoostingClassifier, KNeighborsClassifier** | Classification models  
| **VotingClassifier**   | Ensemble classifier combining multiple models                                

---

## 🧠 Workflow Summary

1. **Data Loading and Cleaning**:
   - Load data from CSV
   - Drop unnecessary columns (`ID`)
   - Handle missing values and convert date columns

2. **Feature Engineering**:
   - Days since customer enrollment
   - Age computation
   - Children categorization (`Kid`, `Teen`, `Both`, `No Child`)
   - Aggregated metrics like `total_mnt`, `total_purchases`, `AverageSpent`, and `Family_Size`
   - Outlier handling using statistical limits

3. **Data Preprocessing**:
   - Categorical column normalization (Education, Marital Status)
   - Scaling with `RobustScaler`
   - One-hot encoding for categorical variables

4. **Exploratory Data Analysis**:
   - Pair plots, scatter plots, line plots, KDE plots, box plots, strip plots
   - Analyzing purchasing behavior and demographics

5. **Classification Model**:
   - Built a soft voting ensemble using Random Forest, Gradient Boosting, and KNN
   - Evaluated using accuracy score

6. **Clustering and Dimensionality Reduction**:
   - KMeans clustering with silhouette analysis
   - PCA for visualization and performance boost
   - Used Elbow and Silhouette methods to determine the optimal number of clusters

7. **Cluster Interpretation**:
   - Visualized clusters using swarm plots, box plots, and radar-like comparative plots
   - Observed purchase patterns, family size, and demographic distribution across clusters

---

## 📈 Key Insights

- Segmentation helps identify distinct customer profiles.
- Spending patterns vary significantly by family size, child presence, and marital status.
- Clustering enhances understanding of group behavior and assists in targeted marketing.

---

## 📌 How to Run

Make sure you have all dependencies installed. You can install them via pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn yellowbrick
```

Then, simply run the Python script in your preferred IDE or notebook environment.

---



Developed by Riakantha Shiva Krishna
