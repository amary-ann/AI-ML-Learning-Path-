# Toxicity Classification
This dataset contains a large number of wikipedia comments that have been classified by human raters for toxic behaviour.

- toxic
- severe_toxic
- obscene
- threat
- insult
- identity_hate

I created a model to predict the probability of each type of toxicity for each comment.

### Problem Statement
> On the internet, there is a lot content. Though, it has benefits , there are some downsides which are dependent on it's usage. For instance, we see a lot of vile comments on social media that can cause a lot of harm to people. 

### Problem Solution
> The purpose of this project is to offer a solution to classify these types of comments using machine learning. This model can then be deployed to filter these comments thereby creating a safer and less negative space for everyone to use

### Process
There are five steps taken to building the model
- <b> Firstly, </b> I imported the necessary libraries and had a quick run through of the data. 
- I took a deep learning approach using tensorflow and so the next step involved me preprocessing the data, which involved tokenizing the comments feature for the model. I also created a pipeline ad created the training, validation and test partitions.
- Following this, I built a sequential model using tensorflow, added different layers to my network and trained the model on the vectorized data.
- Next, was the prediction phase where I predicted a sample text as well as the test partition created earlier.
- Finally, I evaluated the model using a few metrics such as precision, recall, and categorical accuracy from tensorflow.


```python

```
