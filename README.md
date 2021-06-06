
# COMP6200 Group Project

#### Group Members: 
* Arth Mukeshbhai Patel (46117253)
* Vaibhav Aggarwal (45516065)
* Gayathri Renukanath Mahendraker(45780307)
* Rakshit Puniani(46167587)

#### Folder: 
* The group folder consists of one dataset folder which has 2 main csv files: googleplaystore.csv and googleplaystore_user_reviews.csv, presentation.pptx, proposal.md and 3 .ipynb files for our data cleaning, sentiment and applying models.

#### Dataset overview:
Dataset: https://www.kaggle.com/lava18/google-play-store-apps
* We have collected our data from Kaggle but The Data was obtained via Kaggle however, Data cleaning is required as there are a lot of unwanted data and also we go for text cleaning and then select to perform the semantic analysis on comments. One of the CSV files also contain sentiment analysis but we perform it again for better accuracy. In project our aim to analyses application’s comments, review and ratings. We are interested in whether there is a relationship between the comments and the reviews of the applications with the ratings. We may also explore the relationships according to features like categories and type (free/Paid applications).


#### Data cleaning:
* For preprocessing, in dataset 1 (File: googleplaystore.csv) : In the dataset there are13 features, such as rating, categories etc. However, all features contain the string data except Ratings. Convert the necessary columns of the dataset like price, category, reviews count, downloads to float. Remove the unwanted and null values from the dataset.

* For pre-processing, in dataset 2 (File: googleplaystore_user_reviews.csv) : In the dataset there are columns of the comments semantic type, subjectivity and polarity and appname. Using the NLTK movies review dataset we train the model and then test our model and update column with new semantic type (positive/negative reviews). And using Textblob library we update subjectivity and polarity of the comments. Remove the unwanted and null values from the dataset.

#### Data visualization:
* For data insights: We have used different types of graphs and plots to find the relationship between different categories. From our datasets we can gather that 93.1% of the total Apps are free while the rest 6.89% of Apps are the paid ones in the Google Playstore. From the graphs, we also gathered, which app category were the most download and which were least. We could also gather which age group category of apps used to receive maximum number of reviews and by sentiment analysis we were also able to find out were most comments positive or negative.


#### Steps  
* For the File Googleplaystore_user_reviews.csv We preprocessed the data and update sentiment, Sentimnet_polarity and sentimnet_subjectivity columns. Wrote a method to generate words as features. We Fetch the training dataset from the NLTK movies data. After we used Naive Bayes Classifier and Logistic Regression to our trained dataset. And check the accuracy score which is nearly same.

* For the File: Googleplaystore.csv We preprocessed the data and convert datasets columns to float which are mandatory to perform analysis.  For converting columns like content and category we use labelencoder(). Last, we perform the different models such as linear regression, random forest regressor and decision tree regressor. And compare the score and f1 values. 

* From the correlation heatmap plot we can see that most of the features do not show strong relation between each other’s.  However, the reviews show the strong relation with installs and follow by the Size. 

#### Conclusion:
* From the comments of the google play apps we can see that the comments shows mostly negative biased. However, we can see that mostly rating around the more than 4 out of 5. So we can say that there is no relationship with the comments and ratings. After performing the models such as linear , random forest and decision tree regression we can notice that the score is not good enough and the mse value is high. As per our aim of the project we can conclude that there is no relationship between the ratings, count of reviews and comments. Moreover, we also notice that reviews effect on the installation of the apps.
