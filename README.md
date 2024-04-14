# Lab2
Interpretation: How do we interpret the accuracy of a machine learning model?
# Model Evaluation and Interpretation

## Overview:
Continuing with our Lab1 logistic regression on student data to predict the likelihood of student withdrawal from courses, I have added certain evaluation metrics in this version. It evaluates the model's performance using various metrics and visualizations. I have added the visuals as well here.

## Data Preprocessing:
- Categorical variables are converted to factors to prepare the data for modeling.

## Model Training and Evaluation:
- The data is split into training and testing sets (80% training, 20% testing) to train and evaluate the logistic regression model.
- The logistic regression model is trained using the `glm` function with the family set to "binomial".
- Predictions are made on the test data, and a confusion matrix is computed to evaluate the model's performance.

## Confusion Matrix Visualization:
- The confusion matrix is visualized as a chart using ggplot2. It provides insights into the model's classification accuracy and errors.
- ![Image Description](https://github.com/mallelaindira/Lab2/blob/main/8446ba03-1824-4e86-a52c-c840069fe1ef.png)
- ![Image Description](https://github.com/mallelaindira/Lab2/blob/main/Screenshot%202024-04-14%20at%2011.56.19.png)

## Sigmoid Curve Visualization:
- A sigmoid curve plot is generated to visualize the distribution of predicted probabilities output by the logistic regression model.
- The curve illustrates the model's confidence in predicting student withdrawals based on their characteristics.
- ![Image Description](https://github.com/mallelaindira/Lab2/blob/main/6b384a4c-bbeb-478a-80af-c7553b6d8d55.png)
- ![Image Description](https://github.com/mallelaindira/Lab2/blob/main/Screenshot%202024-04-14%20at%2011.58.42.png)

## Model Performance Metrics:
- Model performance metrics including accuracy, precision, recall, F1 score, and specificity are extracted from the confusion matrix and visualized as a bar chart.
- These metrics provide a comprehensive assessment of the model's ability to classify students into withdrawn and non-withdrawn categories.
- ![Image Description](https://github.com/mallelaindira/Lab2/blob/main/f95b37f7-4549-45af-b691-37145f307f30.png)
- ![Image Description](https://github.com/mallelaindira/Lab2/blob/main/Screenshot%202024-04-14%20at%2011.58.50.png)

## ROC Curve and AUC:
- The ROC curve is computed using the `pROC` package to evaluate the model's ability to discriminate between positive and negative classes.
- The AUC (Area Under the Curve) value is calculated to quantify the overall performance of the model.
- ![Image Description](https://github.com/mallelaindira/Lab2/blob/main/759c4e74-4924-476f-ae94-f9340eec099a.png)
- ![Image Description](https://github.com/mallelaindira/Lab2/blob/main/Screenshot%202024-04-14%20at%2011.58.57.png)

## Conclusion:
This simple code demonstrates the sequential steps followed viz training, evaluating, and interpreting a logistic regression model for predicting student withdrawals. Through visualizations and performance metrics, it offers insights into the model's effectiveness and aids in understanding its predictive capabilities.
