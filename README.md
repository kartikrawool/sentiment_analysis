# Sentiment Analysis of Covid-19 Tweets

### Problem Statement
Sentiment analysis is contextual mining of text which identifies and extracts subjective information in source material.
Bearing pertinence to the situation of the coronavirus across the world, there had been a surge in the usage of online platforms and social media sites. One such site, Twitter, most popularly known for its limited sized tweets, had been one of the major platforms where people, government, and a lot of others can communicate effectively and express their opinions.
The project aims to build a model that can accurately disseminate an understanding of the sentiments of people through only the tweet data.

### Dataset
Selected the set of Tweet IDs from  a github repository to get the tweets pertaining to COVID-19 from January to May 2020. 
Extracted tweets from Tweet IDs using Twarc command line tool which enables using Twitter API with ease in Python
The extracted dataset contains 90540 tweets with over 34 features each.

### Data Preprocessing
The filtered tweet’s dataset consisted only of the full_text of the tweets and 90540 rows over which sentiment analysis is to be conducted. 
As a preliminary step, our first instinct was to filter out tweets from the English language only.   

The following preprocessing steps were undertaken:
* Converting the tweet’s text to lowercase 
* Removing punctuations – any punctuations do not add improvement in extracting the sentiments of the tweet
* Removing hash symbols – hashtags contain information about the latest ongoing trends but the hash symbols in themselves can be filtered out to make the tweet’s text more concise
* Eliminating the twitter handles mentioned in the tweet beginning with ‘@
* Eliminating the ‘rt’ i.e. retweet status from the tweets –
* Removing URLs from the tweet 

Before:
> RT @treasonstickers: .@realDonaldTrump when are you going to visit and embrace the people in the US with Coronavirus? https://t.co/lEvq3S4iâ€¦
After:
> when are you going to visit and embrace the people in the us with coronavirus 

