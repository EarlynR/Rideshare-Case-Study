# Ride Share Case Study 

## Objective 

In 7 hours, create and present the best algorithm that presents churn prediction.

## Background 

Company X, a ride sharing company, is interesting in predicting churn so its marketing department can effectively market to 'at-risk' customers. This project has deep roots in business. Even though, my team member and I have to create an algorithm, we must be wary of profits and costs. 

## Data and Our Feature Engineering 

My team was given a dataset that had 12 variables but to make our model more robust, we performed feature engineering and added variables to our model, totaling up to 41 features. 

## Model 

Once our feature engineering phase was over, we proceeded with creating a model. Due to the high number of variables, we opted to use Sklearn's Random Forest Classifier. 

Since there are many hyper-parameters to account for, we used Sklearn's Grid Search to determine the following: 
-minimum samples per leaf
-minimum samples for split
-max depth 
-max leaf nodes
-criterion

Among all these parameters to tune, the best criterion was entropy and maximum number of leaf nodes caps out at 4096.

## Results

We used Sklearn's accuracy score to determine the efficacy of our model. The best score was 0.78%!