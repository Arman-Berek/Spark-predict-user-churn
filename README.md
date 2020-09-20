# Spark Predicting User Churn

### Install
This project requires **Python 3.x** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [Spark](https://spark.apache.org/downloads.html)
- [PySpark]('https://pip.pypa.io/en/stable/installing/')

### Overview
In this project, I user PySpark to predict user churn for a music streaming service similar to Spotify using large datasets. First I predicted on my local machine using a smaller subset of the data, before I use the full 12GB dataset with a spark cluster on Amazon Web Services. I defined churn as the event where a user canceled their accounts. After picking which features I will use for my training set and scaling the data, I then used Spark MLlib to train a variety of models on and after finding the best performing model using the f1 score as a metric, I hypertuned its parameters to look for improvements. The final model I used was Gradient Boosted Trees Classifier and it performed with an f1 score of 0.67.

###
