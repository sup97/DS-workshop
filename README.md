# DS-workshop
Data scraping workshop FA 2019

This workshop will allow participants to scrape Twitter data using keywords or username within specified time frame.
With the scraped data, the workshop will clean and analyze the text data if time allows.

We will be using "GetOldTweets" by Jefferson-Henrique to collect Twitter data.

## Preparation
Before we start the workshop, let's make sure that everyone has Python on their computer.
We will be using Python 2.7
If you don't have Python on your computer, please follow the link and download https://www.python.org/downloads/

After you donwload the Python, please download the files onto your computer and move the file to "Documents".

Then we will open "terminal" OR "PowerShell".
We will move our location to where we downloaded the files.
You can type "cd LOCATIONAME" to move to the location.
Let's move to "GetOldTweets-python-master" folder.

    cd Documents/DS-workshop-master/GetOldTweets-python-master

When at the location, type "ls" or "dir" to see the list of files in the directory.
You should be able to see "Exporter.py".

Type and enter "python" on your command line to see which version you have. If you have version 3, please try the below:
    
    conda create -n python2p7 python=2.7
    source activate python 2p7
(You can deactivate Python 2 by "source deactivate")

If python does not run at all on your Powershell, please refer to following :https://www.quora.com/Why-wont-Python-work-in-PowerShell-for-me

## Collect tweets
We will first install required packages
Type the following in your command line:

    pip install -r requirements.txt
    
If pip is not recognized, please try following: https://pip.pypa.io/en/stable/installing/
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
