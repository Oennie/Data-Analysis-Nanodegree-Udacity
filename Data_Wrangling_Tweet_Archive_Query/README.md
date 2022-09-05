## Reporting: wrangle_report

### Introduction

The data wrangling project focused on going through the whole data analysis process from gathering the data to cleaning, analyzing it and finally visualizing insights from the data. The data used is based on a Twitter account, _WeRateDogs_ which rates dogs from a humorous point of view.


I went through the following process:
1. Gathering data

2. Assessing data

3. Cleaning data

4. Storing data

5. Analyzing and visualizing data

6. Reporting

### #1 Gathering Data

I went ahead to collect the data needed for this analysis from three sources:
* WeRateDogs Twitter archive file at hand provided by Udacity with tweets about random dogs.
* An image prediction of the dog breed file to be programmatically downloaded from the Udacity servers.
* Querying Twitter’s API using the Tweepy library to get additional information on the tweets like favourite and retweet counts.


### #2 Assessing Data

I visually and programmatically assessed the datasets to understand them. I also looked for quality and tidiness issues so as to get them cleaned and ready for anaalysis and visualization.

Here are the issues I identified from the different datasets:

#### Quality issues
**`tweet_archive`**

1. Retweets are present, want only original tweets

2. Multiple null variables in different columns 

3. Null values represented as none in doggo, floofer, pupper, puppo columns

4. Incorrect data type for timestamp

5. 23 rows with denominator != 10

6. Dog names like "None", "a"

**`image_predictions`**

1. Duplicate variables present in jpg_url

2. Inconsistent dog name format in p1, p2, p3 columns 

3. Non-descriptive column names (p1, p2, p3, p1_conf, p2_conf, p3_conf)

4. A number of tweets that do not refer to dog ratings

#### Tidiness issues
1. Information on the tweet are in 3 tables

2. Text column contains repetitive information

3. 4 variables contained in 4 columns (doggo, floofer, pupper, puppo)

### #3 Cleaning Data
In this phase I cleaned all the issues stated in the assesing data stage. I used the `Define-Code-Test` approach to cleaning data.

I fixed all the issues within the datasets using functions from the pandas library. I was left one clean and tidy dataset as I merged all tweet information into one dataframe.

### #4 Storing Data
After gathering, assessing and cleaning the data, it was then saved in a CSV file (master dataset) named `twitter_archive_master.csv`.

### #5 Analyzing and Visualizing Data
My approach to analysis and visualization was to ask a question and then try to answer the question with the data and visualize it.

These are the insights generated during this stage:
* The most common dog breeds are: _Golden Retriever, Pembroke, Labrador Retriever, Chihuahua, Pug, Pomeranian, Toy Poodle, Malamute, Chow and French Bulldog_

* The most common dog names are _Cooper, Charlie, Oliver_

* There seems to be a positive between correlation retweet and favorite counts

* The number of retweets and favourite counts increases over the years

### #6 Reporting

I created 2 documents to describe my wrangling efforts and communicate insights generated from the datasets
