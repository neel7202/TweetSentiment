# TweetSentiment
Many people around the world have been quarantining at home due to the coronavirus. This project aims to see how users on Twitter have been handling being locked at home, with the second component involving the Google Maps API which will show each country’s average tweet sentiment.

# My Work
Working on this was an amazing experience for me. I did not have much experience with API's before so I continued to learn and research as I continued on with the project. This however, brought upon me a few challenges. The largest struggle for me was familiarizing myself with APIs, and specifically the Twitter API. I read up on different functions, capabiilties and limits of the Twitter API I was using. I decided to use the searchTwitter() function as my main way to obtain relevant data from Twitter. 

I decided to quantify twitter senitment by taking the average number of retweets of anxiety-related tweets for each hour group. While doing this, I experienced a lack of both control and quantitiy of extraction from the Twitter API. I frequently received errors due to regulation of the number of tweets I could extract and thus had to use a very limited sample size (100 per day). Moreover, I wanted to extract the same number of tweets for each hour in the data, but could not figure out a way to do this either. Although the y variable is averaged (total rewteets/number of tweets) to rid this disparity in my graph, I lost some consistency in my data. A similar experience occurred to me originally when I only included one searchTwitter() function in my code, until I realized that the only data I was getting was from one day. To ensure all days were equally represrented, I included 7 searchTwitter() functions, one for each day. However, I did not find it practical do this for each hour in each day as that would call for 24 * 7 searchTwitter() functions. Instead, I set the resultType parameter to "popular" to get the most popular tweets over the course of the last week instead of the most recent ones.

If I had more time, firstly, I would have improved upon my time-series graph. More specfically, I would include a greater number, or a more comprehensive metric of twitter sentiment. One idea I have is to measure the number of times the word "anxiety" is mentioned, or the number of other words of negative mental haelth. I would use this to create the variables - "numAnxiety" and "numRelated" - which could be used in addition with the currently used "avgAnxiousTweets" using facet-wrao to represent the relationship between twitter sentiment and time more accurately. 

Secondly, I would have gotten to the second part of the project, which was to create the world map using the Google Maps API. I simply did not have time to get to this, but am looking forward to pursuing this in my own free time as a personal project.


