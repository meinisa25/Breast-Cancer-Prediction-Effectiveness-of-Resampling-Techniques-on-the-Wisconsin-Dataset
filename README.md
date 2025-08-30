# **Breast Cancer Prediction: Effectiveness of Resampling Techniques on the Wisconsin Dataset**

---

## 📱 **About the Project**

This project focuses on evaluating the **effectiveness of resampling techniques** (Holdout, Cross-Validation, and SMOTE) in improving the performance of predictive models on the **Wisconsin Breast Cancer dataset**.  
Breast cancer is one of the most common cancers worldwide. Accurate prediction of whether a tumor is **benign** or **malignant** is crucial for early detection and treatment. By applying **resampling methods** and **Logistic Regression**, this project aims to improve prediction reliability and handle imbalanced data.  

---

## 📋 Dataset

- **Source**: Wisconsin Breast Cancer Dataset (UCI Machine Learning Repository).  
- **Samples**: 569 patient records.  
- **Features**: 30 features (e.g., `compactness_mean`, `area_mean`, etc.).  
- **Target**: Diagnosis (Malignant / Benign).  

---

## 📂 Methodology
The data analysis was carried out using RStudio with the application of various resampling techniques (Holdout, Cross-Validation), standardization (Z-Score), oversampling (SMOTE), and Receiver Operating Characteristic (ROC) 
analysis

1. Import dataset and preprocess (`diagnosis` → binary response).  
2. Define classification task (`TaskClassif$new()`).  
3. Train Logistic Regression model using **MLR3**.  
4. Evaluate with **Holdout** and **Cross Validation**.  
5. Apply **Z-Score Standardization** and **SMOTE** for class balance.  
6. Measure performance with **Accuracy, Confusion Matrix, ROC-AUC**.  
7. Visualize results using `autoplot()` (histograms, boxplots, ROC curve).
   
---

## 🖥 Tools & Libraries

![RStudio](https://img.shields.io/badge/-RStudio-75AADB?style=flat&logo=rstudio&logoColor=white)  
![R](https://img.shields.io/badge/-R-276DC3?style=flat&logo=r&logoColor=white)  
![mlr3](https://img.shields.io/badge/-mlr3-1A73E8?style=flat&logo=r&logoColor=white)  
![caret](https://img.shields.io/badge/-Caret-FF6F00?style=flat&logo=r&logoColor=white)  
![SMOTE](https://img.shields.io/badge/-SMOTE-8E44AD?style=flat&logo=python&logoColor=white)  
![Data Visualization](https://img.shields.io/badge/-Visualization-FF5733?style=flat&logo=r&logoColor=white)  

---

## 📊 Results

- **Holdout**: Logistic Regression achieved ~90% accuracy.  
- **Cross Validation**: Accuracy improved to **93.32%**, showing more reliable performance.  
- **ROC-AUC**: Achieved **91.15%**, indicating strong discrimination ability between benign and malignant tumors.  

✅ Cross Validation proved more effective than Holdout, while SMOTE improved class balance.  
