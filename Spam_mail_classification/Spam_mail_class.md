# Spam Classification 
I created a model for the purpose of distinguishing between spam and ham emails in this project. 

The dataset can be found on kaggle at: https://www.kaggle.com/datasets/veleon/ham-and-spam-dataset

The data contains two features:
- emails
- spam : the value 1 represents spam, while 0 indicates non-spam (also known as ham).

<h2>Actions Taken</h2>
The project was executed through a series of planned and organized steps, aimed at achieving the desired outcome.

- The data obtained from the aforementioned source consisted of raw text files. Therefore, the initial step was to combine the individual files into a more appropriate dataframe format.

- Subsequently, I proceeded to import the required libraries and imported the combined files, which were saved in CSV format, into a dataset.

- The next step involved inspecting the data for any inconsistencies or anomalies. During this assessment, I observed that the emails were in a raw format and required processing to extract the plain text. This involved me using the email library and creating a loop to extract the plain text for each email entry.

- Afterwards, I performed text preprocessing tasks. This involved creating a function 'preprocess_email' to clean and tokenize the email text using NLTK library. Finally, the processed text was rejoined to produce the final result.

- Next, I split the dataset into training and testing sets using train_test_split function, then used scikit-learn's CountVectorizer and TfidfTransformer to vectorize the text data into numerical features that the logistic regression model can use. The CountVectorizer creates a bag-of-words representation of the text data, and the TfidfTransformer transforms the counts into TF-IDF features.

- Then, I trained a logistic regression model using LogisticRegression class. Here, I performed some hyperparameter tuning using GridSearchCV to get the best C hyperparameter value for the model. This ensures a high accuracy for the model.

- To ensure that the model was not overfitting, I conducted cross-validation using the cross_val_score function from the scikit-learn model_selection library.

- Lastly, I created a wordcloud for a selection of spam and non-spam (ham) emails.

## Limitations

It was difficult to identify clear factors such as text, that determine whether an email should be classified as spam or not.
