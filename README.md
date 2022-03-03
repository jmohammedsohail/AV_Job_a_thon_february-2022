# AV_Job_a_thon_february-2022

**Problem Statement:-**

ABC is an online content sharing platform that enables users to create, upload and share the content in the form of videos. It includes videos from different genres like entertainment, education, sports, technology and so on. The maximum duration of video is 10 minutes.

Users can like, comment and share the videos on the platform.

Based on the user’s interaction with the videos, engagement score is assigned to the video with respect to each user. Engagement score defines how engaging the content of the video is.

Understanding the engagement score of the video improves the user’s interaction with the platform. It defines the type of content that is appealing to the user and engages the larger audience.

**Objective:**
The main objective of the problem is to develop the machine learning approach to predict the engagement score of the video on the user level.

Data Dictionary
You are provided with 3 files - train.csv, test.csv and sample_submission.csv

The list of features in the dataset is given below:

| **Variable** |	**Description** |
|----------|---------------|
| row_id	| Unique identifier of the row|
| user_id	| Unique identifier of the user
| category_id |	Category of the video|
| video_id |	Unique identifier of the video |
| age |	Age of the user|
| gender |	Gender of the user (Male and Female)|
| profession|	Profession of the user (Student, Working Professional, Other)|
|followers |	No. of users following a particular category|
| views |	Total views of the videos present in the particular category |
| engagement_score |	Engagement score of the video for a user |


**Acknowledgements :**
https://datahack.analyticsvidhya.com/contest/job-a-thon-february-2022/?utm_source=datahack&utm_medium=navbar#LeaderBoard

**My Approach:**

1.	I have targeted the problem as a regression analysis and used Xgboost regressor machine learning algorithm with RandomizedSearchCV  to build my final model.
2.	For data pre-processing I checked for missing values, looked for correlation in  problem, Using label Encoder converted Categorical data into numeric form.

3.	Before reaching my final model, I have used Random forest and Gradient boosting algorithms, however Xgboost gave a bit better results as compared.
Fine tuning and using extracted column played a crucial role in getting a descent model and score of 0.3105129944 in Public Leaderboard & 0.309420472528165 in Private Leaderboard.


