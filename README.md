# Manufacturing Defect Detection

This project focuses on building a machine learning model to accurately detect defective ball bearings in a manufacturing environment. The aim is to improve quality assurance processes by addressing class imbalance and leveraging advanced modeling techniques.

## Table of Contents
- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Steps to Run](#steps-to-run)
- [Results](#results)
- [Insights](#insights)
- [Future Work](#future-work)
- [Contributors](#contributors)

## Project Overview
This project involves analyzing a dataset with 230,000 samples and 30 predictors to classify ball bearings as defective (`1`) or non-defective (`0`). One of the main challenges was handling the significant class imbalance, as defective samples constituted less than 1% of the dataset.

### Objectives:
1. Develop a robust classification model to detect defective ball bearings.
2. Handle class imbalance using resampling techniques.
3. Optimize model performance metrics such as accuracy, sensitivity, and specificity.

## Key Features
- **Data Standardization**: Scaled all predictors to minimize bias.
- **Visualization**:
  - Histograms to examine data distribution.
  - Heatmaps to analyze feature correlation.
  - Scatter and violin plots for feature relationships.
- **Resampling Techniques**:
  - Random Oversampling
  - Random Undersampling
  - Synthetic Minority Oversampling Technique (SMOTE)
- **Model Experiments**:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Support Vector Machine (SVM)

## Technologies Used
- **Python**: For data preprocessing, visualization, and machine learning.
- **Scikit-learn**: For machine learning models and resampling techniques.
- **Pandas/Numpy**: For data handling and manipulation.
- **Matplotlib/Seaborn**: For data visualization.

## Dataset
- **Source**: Provided for the project.
- **Size**: 230,000 samples with 30 predictors.
- **Data Issues**:
  - Significant class imbalance: ~229,541 samples for the majority class (`0`) vs. 458 for the minority class (`1`).
  - High feature variability requiring standardization.
- **Link to the Dataset**: https://drive.google.com/drive/folders/1m7t8FYqiy5aiJjYbQixcz-2BvuRepupH?usp=drive_link

## Steps to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/aletinithin228/manufacturing_defect_detection.git
2. Ensure all dependencies listed in requirements.txt are installed.
3. Use Jupyter notebooks or equivalent tools to:
4. Preprocess the dataset.
5. Train and evaluate models.
6. Visualize performance metrics.

## Results
- **Logistic Regression**:
  - Accuracy: 99%
  - Sensitivity: 85.06%
  - Specificity: 99.99%
- **Decision Tree**:
  - Accuracy: 96.78%
  - Sensitivity: 91.95%
  - Specificity: 99.99%
- **Random Forest (Oversampled)**:
  - Accuracy: 99.99%
  - Sensitivity: 87.35%
  - Specificity: 99.99%
- **Support Vector Machine (SVM)**:
  - Accuracy: 98.55%
  - Sensitivity: 91.30%
  - Specificity: 99.98%
## Insights
- Resampling Success: Techniques like SMOTE and random oversampling significantly improved minority class detection.
- Model Performance: While Logistic Regression and Decision Tree models performed well, SVM provided the most balanced results between sensitivity and specificity.
- Feature Importance: Predictor X30 was identified as a key feature influencing classification outcomes.
## Future Work
- Optimize SVM kernels to further enhance sensitivity and specificity.
- Experiment with hybrid resampling techniques combining SMOTE and undersampling for a more balanced dataset.
- Explore ensemble models like Gradient Boosting and XGBoost for better handling of imbalanced data.
- Implement deep learning approaches to tackle complex feature relationships.
## Contributors
- Dedeepya Vesangi: Data preprocessing and resampling.
- Harshitha Manaswini Vadavalli: Performance analysis and reporting.
- Nithin Aleti: Model implementation and hyperparameter tuning.
