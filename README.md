# 📋 Play-Store-App-Review-Analysis---Capstone-Project
EDA Capstone Project
![google-play-suppression-applis](https://user-images.githubusercontent.com/103633582/183971679-4423706d-2ddd-4630-9f63-ba7e3517a347.jpg)
--------------------------------------------------------------------------------------------------
## 📋 Introduction
Play Store is a platform from where a user can download apps and rate those apps. In this project I look into the play store app data and the review data and did the analisys to find the improtant features that could help in customer engagement in app

 This Project approach will be :
* Loading Libraries and Dataset
* Data Exploration
* Data Cleaning
* Data Preparation
* Data Visualization
* Analysis Summary
------------------------------------------------------------------------------------------------
## 📋 Loading Libraries and Dataset
I loaded the necessary libraries for the analysis, in which we used Libraries like **Numpy for numerical operations and for n-dimensional arrays**, **Pandas for Data Manipulation and Analysis** and **Matplotlib and Seaborn for Data Visualization**.

I loaded two dataset i.e. Play Store Data and User Review. Play Store Data consisted of columns that were related to the apps like **app size**, **number of installs**, **app category**, **app name**, etc. and User Review consisted of columns like **app name**, **translated review**, ***sentiment*, etc. I loaded the data using the read_csv() function of the Pandas library.
--------------------------------------------------------------------------------------------------
## 📋 Data Exploration
In this step I explored the previously loaded datasets and tried to find some insights from the data. I found that Play Store Data had 1 column with float datatype and 12 columns with object datatype and User Reviews had 2 columns with float datatype and 3 columns with object datatype. I used the functions like head(), tail(), info(), describe(), etc. that help us to explore the data and understand the data.
---------------------------------------------------------------------------------------------------
## 📋 Data Cleaning
In this step I looked for null and missing values by using isnull() and sum() functions on the Play store data and user reviews dataset. I found that Play store data had about 1473 null values in Ratings column, 1 null in Type and Content_Rating columns each and 3 null values in Android_Ver column and User reviews had about 26868 null values in Translated_Review column and 26863 null values in Sentiment, Sentiment_Polarity and Sentiment_Subjectivity columns each. I handled these null by either replacing them or removing the rows that consisted these null values.
-----------------------------------------------------------------------------------------------------
## 📋 Data Visualization
Finally I used Matplotlib and Seaborn to plot to understand the data and find insights in the data. The plots that were used are bar plots, pie plots, scatter plots, etc. 
From these we were able to draw conclusions that would help to know the important features for app engagement.
-----------------------------------------------------------------------------------------------------
## 📜 Conclusion
* The Google Play Store Apps report provides some useful insights regarding the trending of the apps in the play store. as per the graphs visualizations shown above, most of the trending apps (in terms of users' installs) are from the categories like GAME, COMMUNICATION and TOOL even though the amount of available apps from these categories are twice as much lesser then the category FAMILY. The trending of these apps are most probably due to their nature of being able to entertain or assist the user. Besides, it also shows a good trend where we can see that developers from these categories are focusing on the quality of the apps.
* Other than that, the charts shown above actually implies that most of the apps having good ratings of above 4.0 are mostly confirmed to have high number of reviews and user installs. There are some spikes in term of size and price but it shouldn't reflect that apps with high rating are mostly big in size and pricy as by looking at the graphs they are most probably are due to some minority. Furthermore, most of the apps that are having high number of reviews are from the categories of SOCIAL, COMMUNICATION and GAME like Facebook, WhatsApp Messenger, Instagram, Messenger – Text and Video Chat for Free, Clash of Clans etc.
* Even though apps from the categories like GAME, SOCIAL, COMMUNICATION and TOOL of having the highest number of installs, rating and reviews are reflecting the current trend of Android users, they are not even appearing as category in the top 5 most expensive apps in the store (which are mostly from FINANCE and LIFESTYLE). As a conclusion, we learnt that the current trend in the Android market is mostly from these categories which either assisting, communicating or entertaining apps.
