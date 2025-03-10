Author: Justin Short  
Date: 2020-09-01  
Class: CECS 457  

# Heart Disease Classifier
This project is a simple classifier that uses sci-kit learn to train a support vector machine to classify whether a patient has heart disease or not. The dataset used can be found [here](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset). The dataset contains 13 features (and 1 target) and 1025 samples. The features are sex, age, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, and thal. The target is the presence of heart disease (0 = no, 1 = yes). The baseline classifier is trained using 80% of the data and tested using the remaining 20%. The classifier is then used to predict whether a patient has heart disease or not. The baseline model performed with an accuracy of 0.81.  

## Model Improvements
The model was improved using grid search to optimize model hyperparameters. The hyperparameters that were optimized were the kernel, C, and gamma. The grid search was originally performed using 5-fold cross validation, but this lead to minimal improvement over the baseline. 10-fold cross validation was then used, which lead to a significant improvement in accuracy. The optimized model performed with an accuracy of 01.0 on the training set and 0.99 on the test set.


## GitHub Repository
The GitHub repository for this project can be found [here](https://github.com/jnshort/heart_disease_classifier).