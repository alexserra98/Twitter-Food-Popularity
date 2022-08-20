# Twitter-Food-Popularity
This project was written for the final exam of the course Introduction to Machine Learning 2021/22 @ Units.
## Summary
The task was to design and implement a machine learning model in order to predict the popularity of tweets about food. We started by retrieving the corpus of tweets using the Twitter API and then we composed the dataset using both raw features as hashtags, day/hour of publishing, ...etc, and information regarding the content of each tweet, retrieved through standard NLP preproccessing routines.    
The metric chosen for assessing the popularity is $$\ln(\frac{\mbox{num of likes} + \mbox{num of retweets}}{\mbox{num of followers}}) $$ and heuristically resonate with the idea that we wanted to reward the intrisic ability of a tweet to catalyze interest regardless of the number of followers of who wrote the tweet.     
We binned the score of probability that we assigned  to each tweet in the training test so that the problem would belong to a classification framework and as statistical models employed for the prediction we picked Random Forest and Gradient Boosting.    
In order to test the quality of our models we then relied on standard metrics as accuracy, F1 score, precision etc..

![scores-log](https://user-images.githubusercontent.com/92575770/185755612-07dd4504-5689-4e1e-ad10-0ec009701e45.png)

