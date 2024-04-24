# Financial-Loan-Analysis Repository

## About

SC1015 Mini-project that utilises data of applicant's demographic and financial information to determine whether a loan should be approved or rejected based on the provided data.

- [Data Extraction, Preparation and Cleaning](https://github.com/Tableunstable/Financial-Loan-Analysis/blob/main/data-extraction-prep-cleaning.ipynb)
  
- [Exploratory Data Analysis and Splitting ](https://github.com/Tableunstable/Financial-Loan-Analysis/blob/main/EDA%20and%20splitting.ipynb)
  
- [Logistic Regression](https://github.com/Tableunstable/Financial-Loan-Analysis/blob/main/Logistic%20Regression%20.ipynb)
  
- [Random Forest](https://github.com/Tableunstable/Financial-Loan-Analysis/blob/main/Random%20Forest.ipynb)



## Problem Definition

- Are we able to predict an applicant's loan approval based on the interesting variables (ex. education, no of dependents) used in the dataset? 
- Which model is the better to use?

## Models Used
1. Logistic Regression
2. Random Forest

## Evaluation
### Model Performance Metrics:
1. **Random Forest**:
  > - Exhibits high accuracy, with average cross-validation scores around 97.86%.
  > - Shows stability and consistency across different data splits, suggesting good generalization.

2. **Logistic Regression**:
  > - Achieves a high AUC score of approximately 0.985, indicating excellent discriminatory power.
  > - Also shows strong performance metrics like accuracy, precision, recall, and F1-score on the test set.

### Model Suitability:
> - **Random Forest** is generally more robust to overfitting, especially with a large number of trees and diverse data. It’s effective in handling complex structural patterns in data, which can be advantageous if the dataset contains a lot of intricate relationships.
  
> - **Logistic Regression** is highly interpretable and performs well in scenarios where the relationships between features and outcomes are approximately linear or when the focus is on the odds ratios of the predictors. The high AUC score suggests that it can effectively rank predictions, which is crucial in many binary classification tasks.

### Computational Efficiency:
> - **Random Forest** can be computationally intensive, especially with large datasets and a large number of trees, potentially leading to longer training times.
  
> - **Logistic Regression** generally requires less computational resources, making it faster to train on smaller or medium-sized datasets.

## Conclusion (TLDR) :
- Both models perform exceptionally well with the PCA-transformed dataset. The choice between Random Forest and Logistic Regression should be guided by the specific needs of application:
> - **For robustness and handling complex patterns:** Choose Random Forest.
> - **For speed, interpretability, and excellent class discrimination:** Opt for Logistic Regression.
- Yes, it is possible to predict loan approval of an applicant given enough data and variables.


## What new knowledge or insights we acquired from this mini project?
- Logistic Regression from sklearn
- Random Forest from sklearn
- Feature engineering
- Principal Component Analysis
- Standard scaler
- Label Encoding
- K-fold cross-validation
- ROC curve and AUC

## References
- Definition for cibil scores : https://www.bankbazaar.com/cibil/cibil-credit-score.html?ck=Y%2BziX71XnZjIM9ZwEflsyCu5g0osYx%2ByXts24P7rMyyj8dAQXRcJsyhnoHA4bhhF
  
- Why use label encoding instead of one hot encoding :
https://www.analyticsvidhya.com/blog/2020/03/one-hot-encoding-vs-label-encoding-using-scikit-learn/

- Standard scaler: 
https://www.geeksforgeeks.org/what-is-standardscaler/ 
https://medium.com/analytics-vidhya/standardscaler-and-normalization-with-code-and-graph-ba220025c054

- Moveable and immovable assets:
https://krestonsa.com/movable-and-immovable-assets/

- Feature engineering:
https://builtin.com/articles/feature-engineering

- Label Encoding:
https://saturncloud.io/glossary/label-encoding/#:~:text=Label%20encoding%20is%20a%20process,used%20for%20analysis%20and%20modelling.

- PCA: 
https://builtin.com/data-science/step-step-explanation-principal-component-analysis#:~:text=Principal%20component%20analysis%2C%20or%20PCA,information%20in%20the%20large%20set.

- K fold: 
https://machinelearningmastery.com/k-fold-cross-validation/

- ROC curve: 
https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc#:~:text=An%20ROC%20curve%20(receiver%20operating,False%20Positive%20Rate
  
