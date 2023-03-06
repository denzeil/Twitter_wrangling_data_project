# Web Scraping: Tweet Archive of weratedogs data analysis
>I will be gathering data from three sources, including downloading file from Udacity, dowloading from url and web scraping from Twitter API.

>The project includes the following parts:

>gathering

>assessing

>Cleaning

>Analysis report for WeRateDogs project

## Gathering
>Wrangling this project was kind of more tricky and time-consuming than I expected but I have learned a lot. The first part of the data wrangling process is gathering. First, I imported the necessary libraries for my assessment, which are pandas, requests and matplotlib. After that, I programmatically downloaded the image predictions file and saved it. I created a Twitter developer account and accessed the API keys which I stored in variables. I imported the tweepy API and json library. I programmatically downloaded the data using the tweepy API which I saved to a json file and converted to a dataframe.


## Assessing
>After gathering, I had 3 datasets to assess for quality and tidiness issues. I read the dataframes and visually the data. Some of the Quality issues I noted in the enhanced_archive table, the Timestamp column was in object format, and columns like retweeted_status_id - retweeted_status_timestamp had missing values. In the data_convert table, there were two columns for id’s, the columns geo to contributors have almost no values, and the column display_text_range is in object form and has a value range from 0. I also did a programmatic assessment by checking the number of columns in each dataset and using the value counts function to check the number of recurring values. According to the project rubric, we only need the original tweets for analysis. Some of the tidiness issues I noticed are the four-dog stage columns were separated instead of being one and merging the three datasets

## Cleaning
>The third part is cleaning. I used a define, code and test approach for each issue I encountered in the assessing part. Some of the issues I dealt with is converting columns in the wrong format like the Timestamp column to date format and dropping columns that had almost no values like retweeted_status_id to in_reply_to_screen_name. I changed the rating denominator to 10 and fixed the tidiness issues by merging the 4 dog breed columns into one and merging all the 3 datasets into one. After cleaning and I saved the new merged dataset to a new csv file called twitter_archive_master.csv.

## Analysis report for WeRateDogs project
>After gathering, assessing and cleaning the Twitter dataset, I had to analyze it and look for insights. Some of the columns that I used in my analysis are Combined_names, name, rating_numerator, retweet_count and favorite_count.

>To begin with, the first question that I posed was, what is the most popular dog breed, after doing the analysis I found out that the most popular dog breed is pupper and the least is floofer as shown in the bar graph below.

>Moving on to the second analysis I conducted, I wanted to find out the most popular dog name, from the bar graph I noted that the most popular dog names Oliver, Penny, Tucker and Cooper are equally popular compared to other dog names. Although some of the tweets didn’t have the dog names as depicted below.

>The third thing that I wanted to know was the highest dog rating. I found out that the highest dog rating was 12 compared to the rest from the pie chart.

>Another interesting insight that I found is the highest retweet and favorite counts which are 69217 and 141431. After taking a good look at the histogram most of the retweet and favorite counts are concentrated on the left.

>From the information, I obtained from the previous analysis, I got intrigued and used the highest retweet count to find out the dog’s breed and rating. I found out that the dog had a rating of 13 which is a bit higher than the most popular rating and the breed was doggo which is less popular than pupper.



## Key Insights for Presentation

