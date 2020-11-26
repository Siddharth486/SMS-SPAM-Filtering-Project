# ML-Spam-Detection-Deployment

![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-blue.svg) ![Python 3.6](https://img.shields.io/badge/Python-3.6-brightgreen.svg) ![Scikit-Learn](https://img.shields.io/badge/Libraries-ScikitLearn-orange.svg)![NLTK](https://img.shields.io/badge/NLTK-coral.svg)

This repository consists of files required for end to end implementation and deployment of Machine Learning Spam Detection web application created with flask and deployed on the Heroku platform.

# Table of Contents
  * [App Link](#app-link)
  * [About the App](#about-the-app)
  * [Deployement on Heroku](#deployement-on-heroku)
  * [Technologies Used](#technologies-used)
  * [Bug / Feature Request](#bug---feature-request)

A glimpse of the web app:
To check our Project click on the below link which is made by the help of Herouku for web application deployment :
https://spamsmsfiltering.herokuapp.com/


• If you encounter this webapp as shown in the picture given below, it is occuring just because **free dynos for this particular month provided by the Heroku platform have been completely used.** You can access the webpage on 1st of the next month.

• Sorry for the inconvenience.

![Heroku-Error](readme_resources/application-error-heroku.png)

## About the App
The ML Spam Detection is a Flask web application which predicts whether the message is a spam or not. SMS Spam Collection dataset from Kaggle was used to classify the messages into 2 classes- Ham(1) and Spam(0) using stemming, Bag of Words model and Naive Bayes Classifiers.

Note:The dataset is an unbalanced dataset and therefore, for this situation the role of Precision becomes quite important.Precision is more focused in the positive class than in the negative class, it actually measures the probability of correct detection of positive values,

Consider the following case scenario -'suppose if the message is not a spam and if it's been predicted by the model as a spam, the consumer is going to miss that message.' So, for this type of unbalanced dataset, precision defined as {TP/(TP+FP)} plays an important role along with accuracy_score. My objective was to reduce the FP(False Positive) value as much as possible for this case and in order to overcome this issue, Naive Bayes classifiers namely, MultinomiallNB and BernoulliNB were implemented to get best accuracy_score and precision_score from the dataset.

The code is written in Python 3.6.10. If you don't have Python installed, you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries :
```bash
pip install -r requirements.txt
```

## Deployement on Heroku
Login or signup in order to create virtual app. You can either connect your github profile or download ctl to manually to deploy this project.

[![](https://i.imgur.com/dKmlpqX.png)](https://heroku.com)

The next step would be to follow the instruction given in the [Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python) to deploy a web app.

## Technologies Used

![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://flask.palletsprojects.com/en/1.1.x/_images/flask-logo.png" width=170>](https://flask.palletsprojects.com/en/1.1.x/) [<img target="_blank" src="https://number1.co.za/wp-content/uploads/2017/10/gunicorn_logo-300x85.png" width=280>](https://gunicorn.org) [<img target="_blank" src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" width=200>](https://scikit-learn.org/stable/) 

## Bug / Feature Request

If you find a bug (the website couldn't handle the query and / or gave undesired results), kindly open an [issue](https://github.com/Siddharth486/SMS-SPAM-Filtering-Project/Issues) here by including your search query and the expected result


## Please do ⭐ the repository, if it helped you in anyway.
