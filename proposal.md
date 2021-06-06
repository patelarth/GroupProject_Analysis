
## Reviewing the downloads of google play store apps and analysis on their rating and comments

* Arth Mukeshbhai Patel
* Vaibhav Aggarwal
* Gayathri Renukanath Mahendraker
* Rakshit Puniani
<img src='https://d35fo82fjcw0y8.cloudfront.net/2019/01/10100854/CleverTap-Premium-Apps-DataStudy-Header-e1551689672716.png' height='250px' width='500px'>

### AIM :

In our project, we aim to analyses application’s comments, review and ratings. We are interested in whether there is a relationship between the comments and the reviews of the applications with the ratings. We may also explore the relationships according to features like categories and type (free/Paid applications). Also, according to the rating and reviews, we predict the usage of the application by the users. We may also explore the relationships of the downloads and other features.

### DATA SET :

We have obtained accurate datasets of play store applications is an automatic process. Our data was obtained via Kaggle however, Data cleaning is required as there are a lot of unwanted data. Also to perform sentiment analysis we have to perform text cleaning on comments. One of the CSV files also contain sentiment analysis but we have to perform it again for better accuracy. 
* check and remove duplicate values
* Drop null values and outliers.
* Perform sentiment analysis on comments or reviews.

#### dataset Source:
https://www.kaggle.com/lava18/google-play-store-apps

As each of these is separate CSV formats, we will have to join them together. There may be some rows with missing values. We may drop those rows or impute the values manually. Linking these different datasets will be necessary for the analysis we want to perform. All of this will require some data preparation and interaction between datasets.


### Analysis Techniques :

We intend to use regression, RFE, k-means, and k nearest neighbour techniques to achieve what has been outlined in the Goals section above. Regression and RFE will be used to determine what factors go towards the k nearest neighbour analysis.

We expect to use Regular expression techniques to format the comments for processing and for the sentiment analysis we expect to use naive Bayes classifier. To predict reviews/likes, we expect to use logistic regression or clustering techniques. We want to use logistic regression on the different categories of comment sentiment to predict the reviews/likes rating on the applications. 


### Project Plan(milestone) :
* Week 10 Complete Data Cleaning and Manipulation
* Week 11 Complete Model building with at least 3 algorithms
* Week 12 Run tests and evaluate the model

