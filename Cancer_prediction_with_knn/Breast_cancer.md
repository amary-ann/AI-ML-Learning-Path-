# Breast Cancer classification
My goal for this project is to use KNN to classify cancer diagnoses. There are two types of diagnoses; Benign(B) and Malignant(M).

I used a dataset obtained from Kaggle, which can be found at https://www.kaggle.com/datasets/nancyalaswad90/breast-cancer-dataset.

The data contained the following features:
1) ID number
2) Diagnosis (M = malignant, B = benign)
3-32)
Ten real-valued features are computed for each cell nucleus:

a) radius (mean of distances from center to points on the perimeter)
b) texture (standard deviation of gray-scale values)
c) perimeter
d) area
e) smoothness (local variation in radius lengths)
f) compactness (perimeter^2 / area - 1.0)
g) concavity (severity of concave portions of the contour)
h) concave points (number of concave portions of the contour)
i) symmetry
j) fractal dimension ("coastline approximation" - 1)

The mean, standard error and "worst" or largest (mean of the three
largest values) of these features were computed for each image,
resulting in 30 features. For instance, field 3 is Mean Radius, field
13 is Radius SE, field 23 is Worst Radius.

<h2> Action Taken</h2>

Data Collection : The breast cancer dataset was obtained from the source (kaggle) and imported into the project environment for further analysis.

Data Preprocessing : Since the dataset was already cleaned, there wasn't much work required in this regard.

Data Exploration : Exploratory data analysis (EDA) was conducted to gain insights into the data and identify patterns, trends, and relationships within the dataset.

Preparation for Model Development : The label was encoded into numerical values that are more appropriate for the model.

Feature Selection : Relevant features that significantly impacted the diagnosis were identified and selected for modeling.

Model Development : The model was trained and tested on the dataset, and its performance was evaluated based on the accuracy of the classification results.

Hyperparameter Tuning with GridSearchCV : Define the k-NN model and the hyperparameters to tune, and initialize the GridSearchCV object with the model and hyperparameters. Finally, fit the GridSearchCV object on the scaled validation data, and print the best hyperparameters found by the tuning process. We can then use the best model to predict on the testing data using predict(). The tuned model was then evaluated based on the accuracy of the classification results.

Cross Validation: This was employed to obtain a more precise assessment of the model's performance.

Conclusion : While the model initially had a high accuracy, its accuracy was further improved through tuning.
