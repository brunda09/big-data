# Churn Prediction for Sparkify
In this project, we look at Sparkify, a fictional music streaming service with a vast user base and an extensive catalog of songs. Sparkify aims to provide users with a seamless and enjoyable music streaming experience. However, like any subscription-based platform, Sparkify faces the challenge of churn. In this project proposal, we present a comprehensive plan to leverage the power of Apache Spark, a fast and general-purpose cluster computing system, to develop a robust churn prediction model for Sparkify.

### Dataset
We have used a dataset from Udacity Data Science nanodegree project (130 MB). The link to the dataset is:[Sparkify](https://udacity-dsnd.s3.amazonaws.com/sparkify/sparkify_event_data.json). The following is a .json file which contains 18 columns.In our dataset, there is a variable called ‘page’ (target variable with supervised binary classification), showing which platform page the event is linked to. Here we have an option called ‘Cancellation Confirmation’, which refers to the company’s confirmation of a customer’s inquiry to cancel their account. Using this page event as our churn definition means that a customer has churned only when they have completely stopped using the service and canceled their account.

### Data Collection
- Load customer data from a .JSON file named “mini_sparkify_event_data.json”.
- Perform data preprocessing tasks like removing the header, handling missing values, converting categorical variables to numeric ensuring that the data is in suitable format for model training and analysis and splitting the data.

### Model Development
- Model Selection: Use machine learning models for churn prediction, including logistic regression, decision tree, random forest, gradient boosted trees, and multilayer perceptron.
- Feature Selection: Can be applied to identify the most relevant features for churn prediction. It can involve analyzing feature importance scores or using dimensionality reduction techniques like PCA.
- Model Training: The code will train each selected model using the training data, fitting the model parameters to the data, and optimizing them to minimize prediction errors.
- Hyperparameter Tuning: Techniques like grid search or randomized search can be applied to find the best combination of hyperparameters for each model.

### Model Evaluation
- Performance Metrics: Use metrics like accuracy and ROC – AUC curve. These metrics measure the model’s ability to correctly predict churn and distinguish between churned and non-churned customers.
- Cross – Validation: It can be used for assessing model generalization and mitigate overfitting. Techniques like K – fold cross – validation can be used to evaluate models on multiple subsets of the data.
- Validation Set: We will reserve a part of dataset as test set to validate model performance on unseen data. It ensures that model performance is not biased by the training data and provides an unbiased estimate of its performance.
- Visualizations: Visualizations like feature distributions, ROC curves and confusion matrices can provide some useful insights and help in decision making.
  
