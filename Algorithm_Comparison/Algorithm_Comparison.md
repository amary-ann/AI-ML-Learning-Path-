# Algorithm comparison with wine quality dataset
For this project, I will utilize a wine quality dataset to model the quality of wine and as well as evaluate the performance of five distinct machine learning algorithms in this classification task. 

You can access the dataset at the following URL: https://www.kaggle.com/datasets/yasserh/wine-quality-dataset 

This dataset pertains to the red variations of the Portuguese wine "Vinho Verde" and provides information on the quantity of different chemical components within the wine, as well as their impact on its overall quality.

#### It contains the following columns: 
Input variables (based on physicochemical tests):
1. fixed acidity
2. volatile acidity
3. citric acid
4. residual sugar
5. chlorides
6. free sulfur dioxide
7. total sulfur dioxide
8. density
9. pH
10. sulphates
11. alcohol

Output variable (based on sensory data):<br>
12. quality (score between 0 and 10)

## Approach
The following steps were taken in the execution of this project to ensure a comprehensive and thorough analysis of the wine quality dataset:

- <a href ='#dc' style = 'text-decoration: none'> Data Collection </a>: The wine quality dataset was obtained from the source and imported into the project environment for further analysis.

- <a href ='#dp' style = 'text-decoration: none'> Data Preprocessing </a>: The dataset was cleaned, checked for missing values, and any inconsistencies were resolved. 

- <a href ='#de' style = 'text-decoration: none'>  Data Exploration </a>: Exploratory data analysis (EDA) was conducted to gain insights into the data and identify patterns, trends, and relationships within the dataset.

- <a href ='#fs' style = 'text-decoration: none'>  Feature Selection </a>: Relevant features that significantly impacted the wine quality were identified and selected for modeling.

- <a href ='#md' style = 'text-decoration: none'>  Model Development </a>: The following different machine learning algorithms were trained and tested on the dataset, and their performances were evaluated based on the accuracy of the classification results:
    1. <p style = 'color: red'> Decision Tree Model: </p> In this algorithm, the data is split into subsets based on a set of rules or conditions until a stopping criterion is met. To avoid overfitting of the model, the parameter 'max_depth' was set to 3 during its creation. This ensured that the tree was not excessively complex and allowed for better generalization to new data.
    
    2. <p style = 'color: red'> Random Forest Model:</p> A random forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting. To ensure the best outcome, the n_estimators parameter was set to 200. 
    
    3. <p style = 'color: red'> Support Vector Machine:</p> It works by finding the optimal hyperplane that separates the data into different classes while maximizing the margin between them. The margin is the distance between the hyperplane and the closest data points from each class. The C parameter is a regularization parameter that determines the degree of error that is acceptable in the training data. Smaller values may result for misclassifications in the data but may lead to better generalization and vice versa. To select the best value of C, a grid search is performed over a range of C values and the final model is fitted with the best value. 
    
    4. <p style = 'color: red'> K-nearest Neighbours:</p> The KNN algorithm works by calculating the distances between the input data point and all the data points in the training dataset. The "k" nearest data points are then selected based on their distances to the input data point. For low error rates and better accuracy, a graph of error rate vs k value is drawn to get the determine the best n neighbor value.
    5. <p style = 'color: red'> Naive Bayes: </p>The basic idea behind Naive Bayes is to calculate the probability of each class given a set of features, and then select the class with the highest probability as the prediction. This is done using Bayes' theorem.
    

- <a href ='#me' style = 'text-decoration: none'>  Model Evaluation </a>: The models' results were analyzed, and their performances were compared using various evaluation metrics to identify the best-performing algorithm.


- <a href ='#cn' style = 'text-decoration: none'>  Conclusion </a> : A conclusive summary of the project's findings and recommendations for future work were presented based on the results obtained from the analysis.

- <a href ='#lm' style = 'text-decoration: none'>  Limitation </a> : Some limitations of the analysis.

<a id = 'cn'></a>
# Conclusion

In conclusion, the <b style = 'color : green'>Random forest model</b> proved to be the best model for this classification problem with approximately 93% accuracy. However, this model did not have the highest number of correct predictions for the positive class (true positive) when checked with the confusion matrix. The SVM model showed the highest number of true positives and also the highest number of false negatives.

<a id = 'lm'></a>
# Limitations

This dataset was not sufficient determine the metrics that define the quality of the wine as it did not have a enough entries as well as high correlation between the quality feature and other features.


```python

```
