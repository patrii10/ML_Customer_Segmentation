# ML Customer Clustering (Customer Segmentation)

This project aims to analyze a wholesale customer dataset to identify patterns and segment customers into different groups.

---

## **Project Description**
Using information about purchases in categories like fresh food, dairy, cleaning products, and others, we performed an exploratory analysis using **Machine Learning** techniques to better understand customer behavior and segment them into different groups. Once these segments are created, we can tailor marketing strategies for each group.

---

## **Main Objective**
The goal is to identify the key characteristics that group customers together, allowing us to make personalized marketing recommendations.

> What are the main purchasing patterns among customers, and how can we segment them?

---

## **Analysis Content**

1. **Introduction**
   - Problem Description: The goal is to segment customers into different groups based on their purchasing patterns.

2. **Initial Hypothesis**
   - It is proposed that customers can be segmented based on their purchases across different categories such as fresh food, dairy, cleaning products, etc.
   - The aim is to identify relationships between different product categories and customer characteristics.

3. **Exploratory Data Analysis (EDA)**
   - Analysis of key variables such as:
     - Purchases in **Fresh**, **Milk**, **Grocery**, **Frozen**, **Detergents_Paper**, **Delicassen**.
     - Relationship of these variables with **Region** and **Channel**.
   - Analysis of the data distribution, identification of outliers, and transformations performed to improve data quality.

4. **Key Findings**
   - Identification of purchasing patterns and customer distribution.
   - Normalization and transformation of the data (logarithmic and scaling) to prepare the dataset for clustering.
   - Creation of customer segments using clustering techniques.

5. **Conclusions**
   - Final reflections on the identified customer groups.
   - Possible marketing or sales strategies based on the segmented groups.

---

## 📌 Dataset  
- **Name**: Wholesale Customers Data  
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wholesale+customers)  
- **Description**: Contains information about wholesale customers and their purchase patterns in various product categories.

---

## **Tools Used**
- **Python**: For data analysis.
   - **Libraries**: Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn.
- **Jupyter Notebook**: Environment for running the analysis.
- **Clustering**: KMeans for customer segmentation.
- **Transformations**: Normalization and logarithmic transformations of the data.

---

## 📂 Repository Structure  
📁 `src/data_sample/` → Sample of the dataset  
📁 `src/img/` → Graphs and visualizations  
📁 `src/notebooks/` → Test notebooks  
📁 `src/results_notebook/` → Final notebook with the model  
📁 `src/models/` → Saved models  
📁 `src/utils/` → Helper functions  

## 🚀 Methodology  
1. **Data Exploration (EDA)**  
2. **Preprocessing and Normalization**  
3. **Clustering Techniques Application**  
4. **Evaluation of Results**  
5. **Conclusions and Future Improvements**
