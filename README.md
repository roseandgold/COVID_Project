# COVID_Project

SIADS 591/592 Milestone Project
Authors: Laura Stagnaro and Ian Byrne

## Data Sources Used
- [John Hopkins Global COVID-19 Time Series](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series)
- [IEEE-Datapot](https://ieee-dataport.org/open-access/coronavirus-covid-19-tweets-dataset)
- [Twitter API](www.twitter.com)

## Data Manipulation Stages
- Manually downloaded the Twitter ID CSV files and Zip files
- Grab a one percent sample for each day (each CSV represented one day of Tweets) one_perc_sample.py
    - This script should be in a directory containing a another directory named 'ieee_data/' as that is the name of the directory it is currently written to loop through.
- Retrieve the full tweets from the Twitter API using the combined Tweet IDs with twitterAPIScript.py
    - For this to work correctly the user will need to have Twitter Developer API credentials. Pass the script the name of the file with the Tweet IDs that was created with one_perc_sample.py, the start index (0 on the first run), and how many ID's you want to populate on that run. After the run is complete the script will output where it left off to be passed as the start argument on the next run. 
- Combine all of the tweet data into one CSV combineTweetCSVs.py
    - Once you have populated all of the Tweet IDs please place those files in a directory called "tweet_data/". After that is done simply running this script should loop through the directory and combine all of the CSVs.
- Grab the bi-grams for each tweet tweetTokenizer.py
    - 
- Tokenize each tweet to get individual words tweetTokenizerSingleWord.py
    - 
- Daily covid case counts by country covidCountsCountryDay.py
    - 
- Total cases per day covidTimeSeries.py
    - 

## Final Project
- For the project presentation to work, the notebook and packages are located in final_project. These will
need to downloaded to the local machine. 
- The data once accessed, should be downloaded to the same directory as those files.
If simply cloning this repository, the CSVs will need to be placed in the final_project folder. From there all code within the final_project directory should work 
as expected. 
