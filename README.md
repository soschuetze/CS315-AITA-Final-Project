# The Characteristics of Advice-Seeking and Giving on Reddit

## Contents of This File
1. Introduction
2. Requirements

### Introduction
Social media continues to expand its uses, including advice-seeking and giving. Reddit, one such platform, provides specific subreddits just for this purpose. Soliciting advice from unknown users, however, can have vastly different reasons and results than usual advice-seeking from friends. Through the classifi- cation and analysis of posts in the subreddit r/AmITheAsshole, this study aims to understand what topics people might want anonymous advice for and how an online forum style of advice- giving potentially changes the type of advice given. Further, as posts in r/AmITheAsshole are given ratings through user com- ments, our study seeks to understand the distribution of these ratinngs. This research will provide broader social commentary on the effectiveness of using this type of outlet for personal ad- vice. To address our hypothesis, we scrape roughly 10,000 posts published between August 1st, 2021, and March 28th, 2022, us- ing the Pushshift Reddit API. After accounting for posts with no comments or deleted posts, roughly 6,000 posts and their nearly 63 million comments remain in our dataset. The findings of our paper offer a more complete picture on the content of r/AITA, in- cluding the most common types and distributions of ratings in its posts. Additionally, the study identifies popular topics discussed in posts, and any correlations between the topic and rating of a post. Finally, the paper discusses conclusions about whether the comment-based voting style of r/AITA leads to any biases.

### Files and Contents
PM2RedditProject_DataCollection.html: This file contains the code used to collect the 10,000 posts from r/AmItheAsshole using the PushShift API. It also contains the code used to collect the 60 million comments and how we added them to the list of comments for each post. We then saved the post dataframe to a csv to be easily accessed in our data exploration.
PM2RedditProject_DataExploration.html: This file contains the initial data exploration. We added a column to the dataset to determine from the comments the overall rating of each post. We explored how many posts there were for each rating. We also performed some initial topic modeling.
PM3_RedditProject_DataExploration.html: In this file, we continue the data exploration done in the previous file. We added a controversy dataset and added posts there that had a deep split in ratings. We then used these posts to create time series plots that showed how ratings in comments changed over time. We also created a t-SNE graph that shows how ratings vary with titles.
PM5RedditProject_DataExploration.html: In this file, we added code that calculated the percent of ratings for each post. We did this for the controversial posts as well. We also fixed our time series plots by correcting the timestamps to just be the times that the comments were posted. This allowed our time series plots to be more accurate. We added more Gensim topic modeling functions which allowed us to graph the breakdown in how many posts mentioned each topic as their dominant topic.

### Requirements
This project requires the following API
[Reddit Pushshift API]: https://github.com/pushshift/api
