# Credit Card Fraud Detection using Machine Learning
## Introduction
Credit Card fraud i.e. unauthorized access of someone’s credit card, is one of biggest problem that financial industries are facing since introduction of card-based payments. Credit Card fraud is one of the biggest sources of revenue loss for payment card industry. In 2018, $24.26 Billion was lost due to payment card fraud worldwide. The United States leads as the most credit fraud prone country with 38.6% of reported card fraud losses in 2018.

Financial institutions use **traditional fraud detection** system.
Some issues with traditional fraud detection system:
*	Requires domain expertise to build and maintain the system.
*	High operating cost for maintenance.
*	Greater Time to market to combat new fraud trends.
## Data Used
* Dataset: [Creditcard Fraud Dataset](https://www.kaggle.com/isaikumar/creditcardfraud)
* Highly **imbalanced Dataset**. Out of 284807 total transactions only 492 transactions are fraudulent i.e. it represents only 0.17% of the entire dataset.
* To maintain the data confidentiality, most of the variables (V1 through V28) were PCA transformed.
## Technology Used
* Python 3
* Jupyter Notebook on Anaconda
## Method Used
* Pandas Profiling for initial Data Exploration.
* Find input features that are most correlated to output class.
* Boxplot to detect & remove outlier.
* Set **Pipeline** to do data transformation using **ColumnTransformer** and **RobustScaler**.
* Average Precision is used for matrix evaluation.
* **GridSearchCV** is used to tune Random Forest, Logistic Regression and Artificial Neural Network Classifier parameters and select the best one.
* Best model's performance test and evaluation.
## Potential Issues
* Dataset is highly imbalanced. This may create problems for model training.
* V1,..,V28 are PCA transformed. No way to carry out visualization for these fields.
* Limited training data may not fully converge ANN model.
## Future Scope
* Random Forest classifier needs to be **calibrated** to achieve good result.
* **Oversampling** the minority class would address imbalance dataset problem.
* Keeping these models **up to date** using latest fraud data is required.
## Reference
* [Artificial Neural Network](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html)
* [Credit Card Fraud Statistics](https://shiftprocessing.com/credit-card-fraud-statistics/)

[Go Back](https://saurabhbiswas1985.github.io/)
