# WE-RATE-DOGS-DATA-WRANGLING-

Gathering Data
The data set used for this project was collected from the tweets of twitter user @dog_rates. Data was gathered using three different methods namely; direct download, programmatic download, and downloading via Twitter API (tweepy).

Direct download
'twitter-archive-enhanced.csv' data was downloaded directly from the internet and then read into a pandas dataframe

Programmatic Download
Data was gotten from a web page using the request library. This is also known as webscrapping. 'image-predictions.tsv' file was extracted from the url page and a tsv file was read into a pandas dataframe

Via Tweepy
Tweepy is the Twitter API which was used to extract 'tweet_json' file from We Rate Dogs twitter feeds. Information extracted includes tweet id, retweet count and Favorite counts

Assessing Data
Data usually comes in messy and untidy, therefore it is important that they assessed for cleaning. Here, I assessed the data programatically and visually. From the assessement, a couple of quality and tidiness issues were discovered, such as;

null observations
wrong datatype classification
tables needing to be merged
unwanted retweeted observations
rating denominators that are not equal 10
missing values ### Cleaning Data The data quality and tidiness issues observed from the data assessement were taken care of in this section. But before cleaning, copies of the original data were made to avoid loosing data by mistake. A couple of cleanings were done here using relevant python functions;
Columns with missing values were removed using the 'drop' function
wrong datatypes were reclassified using the 'astype' function
tables are combined using 'merge' function
All rating denomintors were set to 10
The cleaned data was then saved as a csv dataframe.
