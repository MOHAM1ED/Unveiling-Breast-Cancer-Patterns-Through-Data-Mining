# Unveiling-Breast-Cancer-Patterns-Through-Data-Mining
This project classifies breast cancer tumors as malignant or benign using data mining, focusing on preprocessing, feature selection, and model training. A Random Forest model delivers high accuracy, with LIME and SHAP enhancing interpretability. These insights provide transparency and support informed decision-making in diagnosis

---
## Table of Contents
1. [Introduction](#introduction)
2. [Data Preprocessing](#data-preprocessing)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Data Visualization](#data-visualization)
5. [Feature Engineering and Selection](#feature-engineering-and-selection)
6. [Model Training and Evaluation](#model-training-and-evaluation)
7. [Model Interpretation](#model-interpretation)
8. [Conclusion](#conclusion)
9. [Future Work](#future-work)
10. [References](#references)

## Introduction
This project aims to analyze and classify breast cancer diagnoses using data mining techniques. Our objective is to classify tumors as either malignant (M) or benign (B) based on features derived from cell nuclei images. Key steps include data preprocessing, feature selection, model training, evaluation, and interpretation.

### Dataset
The dataset consists of features extracted from digitized images of fine needle aspirates (FNA) of breast masses. Key columns include:
- **id**: Unique identifier for each patient (not used in modeling)
- **diagnosis**: Target variable (M = malignant, B = benign)
- **Unnamed: 32**: Column containing NaN values (removed during preprocessing)
- **Feature columns (30)**: Describe characteristics of cell nuclei in images

## Data Preprocessing
- **Data Loading**: Load and inspect data.
- **Data Cleaning**: Drop unnecessary columns (`id` and `Unnamed: 32`) and encode the `diagnosis` column.
- **Encoding**: Convert categorical variables to numeric format.

## Exploratory Data Analysis (EDA)
- **Statistical Summary**: Overview of data distributions and central tendencies.
- **Target Distribution**: Analyze the balance of diagnosis classes.

## Data Visualization
- **Feature Visualization**: Analyze distributions using violin plots, box plots, swarm plots, and correlation heatmaps.
- **Correlation Analysis**: Identify highly correlated features to guide feature selection.

## Feature Engineering and Selection
1. **Standardization**: Ensure equal contribution of each feature.
2. **Feature Selection Techniques**:
   - Correlation-Based Feature Selection
   - Univariate Feature Selection (Chi-Squared)
   - Recursive Feature Elimination (RFE) and RFECV
   - Tree-Based Feature Selection (Random Forest)

## Model Training and Evaluation
- **Model**: Random Forest classifier.
- **Evaluation Metrics**: Accuracy, confusion matrix, precision, recall, F1-score, and ROC-AUC.

## Model Interpretation
We used Explainable AI (XAI) methods to interpret the model:
- **LIME**: Highlights key features influencing individual predictions.
- **SHAP**: Explains feature impacts across the dataset, ensuring consistent interpretation.

## Conclusion
We successfully classified breast cancer tumors with high accuracy and interpretability. Using LIME and SHAP, we enhanced model transparency and trustworthiness. Key findings include:
- Balanced dataset for malignant and benign cases
- Improved model performance through feature engineering
- Insights into model decision-making

## Future Work
- Experiment with additional machine learning models
- Explore deeper feature engineering techniques
- Implement more advanced XAI methods for better interpretability

## References
1. ["Explainable AI for Medical Data: Current Methods, Limitations, and Future Directions"](https://dl.acm.org/doi/pdf/10.1145/3637487)
2. ["Breast Cancer Wisconsin (Diagnostic) Data Analysis"](https://link.springer.com/chapter/10.1007/978-3-030-82099-2_27)
3. ["Breast Cancer Wisconsin (Diagnostic) Data Set"](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)
4. Data Mining course lectures

--- 
