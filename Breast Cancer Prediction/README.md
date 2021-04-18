# Breast Cancer Prediction by Machine Learning
## Introduction
Breast Cancer is the 2nd most common cancer in women. But, on rare scenario can also happen to men. It is 2nd leading cause of deaths of women after lung cancer. A fine needle biopsy is an effective tool in evaluating and diagnosing suspect lumps or masses. With early diagnosis of breast cancer, patients can be isolated for early treatment for a better chance of survival.
Early detection of disease has become a crucial problem due to rapid population growth in medical research in recent times.

My aim is to develop a **classification model** that will identify breast cancer using the FNA diagnosis label with **higher accuracy**. This model will be great for **predicting cancer in advance**, because classification algorithms make boundaries between data points classifying them as a certain group, depending on their characteristics matched against the model’s parameters.

## Data Used
* Dataset: [UCI Irvine machine learning repository](http://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)
           [Breast Cancer](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data) 
* **30 input features**. The mean, standard error and "worst" or largest (mean of the three largest values) of main features like radius, texture, Perimeter etc.  features were computed for each image, resulting in 30 features.
* Dataset is not much imbalanced. Out of total 569 sample, 357 of data samples labelled as B (benign - no cancer) and 212 of data samples labelled as M (malignant - cancer).
## Technology Used
* Python 3
* Jupyter Notebook on Anaconda
## Method Used
* Pandas Profiling for initial Data Exploration.
* Target variable values have translated from B (benign) to 0 and M (malignant) to 1. Target variable ‘0’ will be treated as no cancer and ‘1’ will be treated as breast cancer.
* Drop correlated features after keeping one from each category.
* **Boxplot** to detect outlier.
* **Z-score** calculation to remove outlier.
* Accuracy and F1-score are used for matrix evaluation.
* Set up pipeline
* **GridSearchCV** is used to tune Random Forest and Logistic Regression Classifier parameters and select the best one.
* Best model's performance test and evaluation.
## Potential Issues
* Limited training data.
* Random Forest classifier are not best suited for skewed class distribution. Our dataset is imbalanced dataset.
## Future Scope
* Random Forest classifier needs to be **calibrated** to achieve good result.
* Production deployment of fully trained model
## Reference
* W.H. Wolberg, W.N. Street, D.M. Heisey, and O.L. Mangasarian. Computerized breast cancer diagnosis and prognosis from fine needle aspirates. Archives of Surgery 1995;130:511-516.
* You, H., & Rumbe, G. (2010). Comparative study of classification techniques on breast cancer FNA biopsy data.
* W.H. Wolberg, W.N. Street, D.M. Heisey, and O.L. Mangasarian. Computer-derived nuclear features distinguish malignant from benign breast cytology. Human Pathology, 26:792--796, 1995.
* Xiong, X., Kim, Y., Baek, Y., Rhee, D. W., & Kim, S. H. (2005, May). Analysis of breast cancer using data mining & statistical techniques. In Sixth International Conference on Software Engineering, Artificial Intelligence, Networking and Parallel/Distributed Computing and First ACIS International Workshop on Self-Assembling Wireless Network (pp. 82-87).

[Go Back](https://saurabhbiswas1985.github.io/)
