# Genre-Detection and Text Analysis

## 1.Abstract
In this group project, we analysed text descriptions of movies and developed a predictive model that can predict whether or not a movie is a comedy. The descriptions/story were used to create textual features of the movie descriptions/story and multiple models were created in order to find the best performing model. 

## 2.Introduction
There is nothing more frustrating than not finding the right movie to watch. Understanding movie descriptions/story could give an insight of the type of genre the movie is. It can be a comedy, romance, horror or another type of film. Sorting through movies by their genre would make it easier for movie viewers to find the movie they want to watch. The goal of this group project is to predict whether or not a movie is a comedy based on the movie description/story.

## 3.Data
The data used for this group project was provided by Dr. Mahyar S Vanghefi. This data consisted of 3 csv files found below: movie_story_student_file.csv, movie_story_evaluation_file.csv and movies.csv.

The movies.csv dataset was used to create a new column to contain the target feature (genres) for movie_story_student_file.csv and movie_story_evaluation.csv.This was done by joining the data on movieid/movie_id. Next, this new column was turned into a binary format and identified 1 for comedy and 0 for non-comedy.
Later in the modeling, Movie_story_student_file.csv is used to train models and find the best performing model and Movie_story_evaluation.csv is used to test the best performing model created with Movie_story_student_file.csv.
In order to turn the unstructured data into structured, word embedding was used. We decided to take this approach because we noticed we had over 100,000 features when we used the count vectorizer method from sklearn. Also, Word embedding seems to be a better approach with dealing with high dimensional data. Regarding word embedding, GLoVe 300d was used as our pre trained word embedding method

## 4.The Model
We chose to use logistic regression, decision tree, random forest and Stochastic Gradient Descent for binary classification of comedy movies. The data was split 70% training and 30% test using train_test_split from sklearn.

## 5. Conclusion
The goal of this group project was to predict whether or not a movie is a comedy based on the movie description/story. And, to use the movie_story_student_file.csv dataset to train different models in order to find the best model for classifying comedy movies; and then using the Movie_story_evaluation.csv data set to further test our best model.

Logistic regression performed the best out of all of the models we trained. At first, we were worried that our initial logistic regression model was suffering from underfitting. This was because we found our accuracy to have a large amount of bias and very low variance but after using this new data set, the accuracy came very close to what it previously was predicting and no issues were found

### For elaborated results check the report included in files.
