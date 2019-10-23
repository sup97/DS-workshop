# DS-workshop
Data scraping workshop FA 2019

This workshop will allow participants to scrape Twitter data using keywords or username within specified time frame.
With the scraped data, the workshop will clean and analyze the text data if time allows.

We will be using "GetOldTweets" by Jefferson-Henrique to collect Twitter data.

## Preparation
Before we start the workshop, let's make sure that everyone has Python on their computer.
We will be using Python 2.7
If you don't have Python on your computer, please follow the link and download https://www.python.org/downloads/

After you donwload the Python, please download the files onto your computer and move the file to Documents.

Then we will open "terminal" OR "PowerShell".
We will move our location to where we downloaded the files.
You can type "cd LOCATIONAME" to move to the location.

When at the location, type "ls" to see the list of files in the directory.
You should be able to see "GetOldTweets-python-master" and "text_analysis.Rmd"
Let's move to "GetOldTweets-python-master" folder.

## Collect tweets
We will first install required packages
Type the following in your command line:

    pip install -r requirements.txt
### Get help use
    python Exporter.py -h
### Get tweets by username
    python Exporter.py --username "PennStateRPTM" --maxtweets 1
### Get tweets by query search
    python Exporter.py --querysearch "penn state RPTM" --maxtweets 1
### Get tweets by username and bound dates
    python Exporter.py --username "PennStateRPTM" --since 2019-09-10 --until 2019-09-12 --maxtweets 1
### Get the last 10 top tweets by username
    python Exporter.py --username "PennStateRPTM" --maxtweets 10 --toptweets

## Move to text_analysis.Rmd
