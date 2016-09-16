
Simple Twitter Scraper
======================


## Setting Up

First, install the tweepy library
```
    pip install tweepy
```
Next, either:
- Click the "Clone or Download" button and download the zip file. Then extract simple_scraper.py from the zip file.
- Install git and clone this repository by entering the following command in a terminal: `git clone https://github.com/srisi/Simple-Twitter-Scraper.git`


Finally, To get these scripts working, you need to jump through some hoops to get twitter api access.
Namely, you need the following:
- Consumer Key
- Consumer Secret
- Access Token
- Access Token Secret

To obtain these keys, do the following:

1. Create a twitter account
2. Go to https://apps.twitter.com/<br>
    Click: "Create an application"<br>
        Here, you can enter placeholder values or whatever you want, e.g.:<br>
        Name: asdf846<br>
        Description: asdfasdfasdf<br>
        Website: http://www.asdf.com

    Click: "Create your Twitter application"<br>
    In the following screen, go to the tab "Keys and Access Tokens

    Copy the Consumer Key and Consumer Secret from "Application Settings"
    Copy the Access Token and Access Token Secret from "Your Access Token"

3. Fill in the following placeholder values at the top of simple_scraper.py with your keys:
    <br>CONSUMER_KEY, CONSUMER_SECRET, ACCESS_TOKEN, ACCESS_TOKEN_SECRET
    <br>Note: each of these keys have to be strings, so you need to surround your keys with quotation marks e.g.
    <br>CONSUMER_KEY = "OEitehociOGe069toeifDotea"

## Tutorial
For a tutorial, look (and run) through the tutorial() function at the end of simple_scraper.py

To run the tutorial, open a terminal, move to the folder with simple_scraper.py and execute `python simple_scraper.py`

## Usage
The easiest way to use simple_scraper.py is to modify the `if __name__ == '__main__':` section at the end of the file and then run the scraper from a terminal using `python simple_scraper.py`. 
<br>For example, to scrape 100 tweets mentioning @realdonaldtrump for the last 10 days and storing them to trump.csv, your main function would look like this:

```
if __name__=='__main__':

    #tutorial() <- adding a # means the line is "commented out" and will not be run
    tweets = scrape_term_by_day('@realdonaldtrump', start_date='2016-09-06', end_date = '2016-09-16', tweets_per_day=100)
    store_tweets_to_csv(tweets, 'trump.csv')
```

