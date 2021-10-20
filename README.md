<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# # football_predictions_final_proyect --- Football Results and Shots Predictions
*Samuel Simeone Sanchez*

*DAFT-MX-2021/10/22*

## Content
- [Project Description](#project-description)
- [Instructions](#instructions)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

## Project Description
The objective of this project was to build a supervised machine learning model capable of predicting the results of a soccer game. Subsequently, it was expanded to be able to predict the result of a shot, that is, if it was a miss or a goal depending on the distance to the goal and the angle of the shot.

## Instructions
- Select a dataset from a public source.
- Create a jupyter notebook where the iterative data analysis process is carried out (cleaning, analysis, EDA, visualization and predictive models).
- The objective of the analysis is to identify the most important characteristics of the data obtained. For this, it is necessary to understand the data and study it in depth. To finally make a predictive model that allows us to answer certain questions posed at the beginning of the project

## Workflow
- The first step consisted of searching for the datasets and scraping the necessary information for the project.
- The second step consisted of understanding the data, in order to know how to proceed when cleaning.
- A new table was built from the data obtained, which will be used in the machine learning process.
- The distributions of our data were analyzed. We saw that we had many outliers, so the LOF method was used to treat them.
- The correlations between our variables were studied.
- A reduction of dimensions was made. For this, the Recusive Feature Elimination method was used to identify the most important parameters of our data.
- Several supervised machine learning models were studied, but the Random Forest model was found to be the best. A grid search was performed to find the best parameters
- Once the model was obtained, several evaluations were carried out such as: the confusion matrix, the recall, f1 scores and the accuracy to know how well our model was behaving.
- Subsequently, the model capable of predicting goals was built. The initial process was the same, but in this case we had non-homogeneous data, that is, a large proportion of shots and a low proportion of goals, so the weights of the variables were used in the model to deal with this problem.
- The rest of the steps are similar to those of the previous model, except that the outliers were not dealt with here, since it did not make sense to do so and a reduction of dimensions was not carried out. What was applied was a Rare Label concoding to be able to transform our categorical data to numerical.
- The notebooks were ordered. Comments were placed on the lines of code and the presentation was made.

## Organization
In this repository we are going to find several files, first we have the .ipynb which are python files that contain the project code. They are separated by scraping, cleaning, visualizations and the machine learning model. On the other hand, we have the data and file folders that contain the different data sets used in this project.

## Links
[Repository](https://github.com/)

[Database1](https://www.kaggle.com/stefanoleone992/fifa-22-complete-player-dataset?select=players_21.csv)

[Database2](https://www.kaggle.com/technika148/football-database)

[Imbalance class weights](https://www.analyticsvidhya.com/blog/2020/10/improve-class-imbalance-class-weights/)

[Fbref](https://fbref.com/en/comps/9/schedule/Premier-League-Scores-and-Fixtures)

[Club ELO](http://clubelo.com/2021-08-20/ENG)

[LOF](https://towardsdatascience.com/anomaly-detection-with-local-outlier-factor-lof-d91e41df10f2)

[Football prediction using statistics from brazilian championship](https://towardsdatascience.com/machine-learning-algorithms-for-football-prediction-using-statistics-from-brazilian-championship-51b7d4ea0bc8)

[Modeling expected goals](https://towardsdatascience.com/modeling-expected-goals-a756baa2e1db)