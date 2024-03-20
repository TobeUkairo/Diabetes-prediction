# Early-diabetes-prediction
This repository hosts a comprehensive machine learning project focused on predicting the likelihood of diabetes in patients based on a variety of influential factors.
# Executive Summary

**Objective**: Create a predictive model to determine if a patient has diabetes or is potentially diabetic.

**Key Findings**: 
- the features “polydipsia” and “polyuria” are critical factors for predicting if a patient has diabetes or is potentially diabetic. 

- The 'age' column appears to exhibit a normal distribution.

- 63% of our patients are male.

- Approximately 42% of our patients had experienced weight loss.

- the following columns were fairly balanced; Polyuria, Polyphagia, Polydipsia, Delayed healing, Partial paresis, itching, visiual blurring.

- Approximately 59% of our patients had experienced weakness.

- 78% of our patients had experienced genital thrush.

- Approximately 24% of our patients had experienced irritalbility.
  
- 38% of our patients had experienced muscle stiffness.
  
- 34% of our patients had alopecia.
  
- 17% of our patients were obese.
  
- The target column was slighly imbalanced with approximately 62% of the patients labelled positive.

**Recommendation**: Focus on acquiring high-value brands and adjust pricing strategies based on age, mileage, and fuel type.


## Data Overview

**Dataset Description**: This dataset contains the sign and symptpom data of newly diabetic or would be diabetic patient.



## Data Preparation

**Transformation**: Applied standard scaler to the X_train dataset and X_test dataset.

**Feature Engineering**: used label encoder to encode all categorical variables.

**Model Selection**: compared between KNN, Decision Tree, Logistic Regression and SVM models.

**Hyperparameter Tuning**: Employed GridSearchCV for optimal parameter selection.

## Model Insights and Interpretation

**Model Performance**:

the logistic regression model performed best out of the models compared. after hyper parameter tuning it was able to predict the target variable with 93.6% accuracy, 95% precision, 95% recall, and an F1-score of 95%

## Results:

The performance of four machine learning models—Logistic Regression, K-Nearest Neighbors (KNN), Decision Tree, and Support Vector Machine (SVM)—was evaluated on a dataset for predicting diabetes. Logistic Regression exhibited a training accuracy of 92.1% and a test accuracy of 91.0%, making it the preferred model due to its balance between training and test performance. KNN showed a slightly lower training accuracy of 91.4% and a test accuracy of 85.9%. The Decision Tree model achieved a perfect training accuracy of 100%, indicating potential overfitting, but performed well on the test set with an accuracy of 97.4%. SVM, however, showed a lower training accuracy of 60.6% and a test accuracy of 66.7%. Further evaluation of the Logistic Regression model with the best parameters (C=1, penalty='l2') resulted in an improved accuracy of 93.6%. Feature importance analysis revealed significant contributions from attributes such as Polydipsia, Polyuria, and Gender, indicating their strong correlation with diabetes prediction.

## Limitations and Future Work

**Limitations**:

slightly imbalanced dataset. 

## Recommendations:

- **Feature Selection**: Given the importance of features such as Polydipsia, Polyuria, and Gender, focus on collecting and refining data related to these attributes to enhance the predictive power of the model. 
- **Model Tuning**: Continue fine-tuning the logistic regression model with different regularization parameters to find the optimal settings for improved performance. 
- **Data Collection**: Consider gathering additional data points or features that may provide valuable insights into diabetes prediction, thereby enriching the dataset and potentially enhancing model accuracy. 
- **Validation**: Validate the logistic regression model on external datasets to assess its generalization capability and ensure robustness across different populations or demographics. 
- **Model Deployment**: Once satisfied with the model's performance, deploy it in a production environment to assist healthcare professionals in early diabetes detection and intervention strategies. Ensure regular monitoring and updates to adapt to evolving patient data and healthcare trends. 
