# SPS-454-Diabetes-Prediction-using-Machine-Learning
## Diabetes Prediction using Machine Learning

### Introduction:
  The Diabetes Dataset contains 8 features and a target feature to predict whether women is suffering from diabetes or not.
  All 8 features are continous features and NaN values are imputed with zero.
  
### Approach:
  1. First I fixed the variable(feature) distribution by using different methods.
  2. As the dataset is small without removing outliers, I fixed the outliers by 1.5 IQR
  3. Then I captured NaN value by creating extra feature and imputed with median value with respect to the target feature.
  4. I trained the SVC Classifier with kernal as 'rbf ' 
  5. I tested the model using roc_auc_score as a performance metric 
  6. By using cross_val_score (cv=5), the model gave mean roc_auc_score  of 0.9351
  7. On test data I got roc_auc_score of 0.8924
