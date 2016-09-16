
Simple Twitter Scraper
======================




## Setting Up

First, install the tweepy library
```
    pip install tweepy
```
Next, either:
- Click the "Clone or Download" button and download the zip file. Then extract simple_scraper.py from the zip file.
- Install git and clone this repository by entering the following command in a terminal: 'git clone https://github.com/srisi/Simple-Twitter-Scraper.git'


To get these scripts working, you need to jump through some hoops to get twitter api access.
Namely, you need the following:
- Consumer Key
- Consumer Secret
- Access Token
- Access Token Secret

To obtain these keys, do the following:

1. Create a twitter account
2. Go to https://apps.twitter.com/
    Click: "Create an application"
        Here, you can enter placeholder values or whatever you want:
        Name: asdf846
        Description: asdfasdfasdf
        Website: http://www.asdf.com

    Click: "Create your Twitter application"
    In the following screen, go to the tab "Keys and Access Tokens

    Copy the Consumer Key and Consumer Secret from "Application Settings"
    Copy the Access Token and Access Token Secret from "Your Access Token"

3. Fill in the following placeholder values at the top of simple_scraper.py with your keys:
    CONSUMER_KEY, CONSUMER_SECRET, ACCESS_TOKEN, ACCESS_TOKEN_SECRET
    Note: each of these keys have to be strings, so you need to surround your keys with quotation marks e.g.
    CONSUMER_KEY = "OEitehociOGe069toeifDotea"
