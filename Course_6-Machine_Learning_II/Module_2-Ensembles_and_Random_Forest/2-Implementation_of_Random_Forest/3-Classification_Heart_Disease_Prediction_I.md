# Classification: Heart Disease Prediction - I

In this segment, you will learn how to implement random forests in Python using the sklearn library. You will experiment with hyperparameters, such as the number of trees and the number of variables considered at each split. 

In this segment, you will be working with the heart disease data to build a random forest model in order to predict whether a person has a heart disease or not. The data lists the results from various tests, which were conducted on patients, along with some other details of the patients.

  
You can download the data set here.

Download [Heart Disease Dataset](heart_v2.csv)

Please note the following:

-   **Heart disease = 0** means that the person does not have heart disease.
-   **Heart disease = 1** means that the person has heart disease.
-   **sex = 0** means that the person is female.
-   **sex = 1** means that the person is male.

You can download the code file for your reference from the link given below as well. Please fill the notebook as you watch the video in order to get more clarity and hands-on practice.

Download [Python Code File](Heart_Disease_Prediction_Random_Forest.ipynb)

Please note that we have not done a lot of feature engineering in order to focus more on building the random forest model. In the forthcoming video, we will load the data and create the train and test data sets. 

**VIDEO**

We have now divided the data set into train and test sets. Even though it is not necessary to keep a separate test set in a random forest model, we will try to evaluate the model on unseen data as well. Now, in the next video, we will build a model using a **RandomForestClassifier()** with some arbitrary parameters for simplicity and better prediction results.

**VIDEO**

You can easily build a random forest model in Python using the RandomForestClassifier(). As part of the process, you looked at some sample trees and must have now understood how the process takes place internally. The two sample trees used in the process are given below.

![Random Forest Heart Disease Prediction](https://i.ibb.co/2jvYT0S/Random-Forest-Heart-Disease-Prediction.jpg)

You also learnt how to fetch the OOB score generated by the classifier in order to understand how the collection of these individual trees performs. In the next segment, you will learn how to tune some hyperparameters using gridsearchcv() in order to make our ensemble model perform better.