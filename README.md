# Python2Twitter
Python2Twitter Streaming project

1. Getting Twitter API keys

To start with, you will need to have a Twitter account and obtain credentials (i.e. API key, API secret, Access token and Access token secret) on the Twitter developer site to access the Twitter API, following these steps:

    Create a Twitter user account if you do not already have one.
    Go to https://apps.twitter.com/ and log in with your Twitter user account. This step gives you a Twitter dev account under the same name as your user account.
    Click “Create New App”
    Fill out the form, agree to the terms, and click “Create your Twitter application”
    In the next page, click on “Keys and Access Tokens” tab, and copy your “API key” and “API secret”. Scroll down and click “Create my access token”, and copy your “Access token” and “Access token secret”.



2. Installing a Twitter library

We will be using a Python library called Python Twitter Tools to connect to Twitter API and downloading the data from Twitter. There are many other libraries in various programming languages that let you use Twitter API. We choose the Python Twitter Tools for this tutorial, because it is simple to use yet fully supports the Twitter API.

Download the Python Twitter tools at https://pypi.python.org/pypi/twitter.





3. Connecting to Twitter Streaming APIs

The Streaming APIs give access to (usually a sample of) all tweets as they published on Twitter. On average, about 6,000 tweets per second are posted on Twitter and you (normal dev users) will get a small proportion (<=1%) of it. The Streaming APIs are one of the two types of Twitter APIs. The other one called REST APIs (we will talk about later in this tutorial), which is more suitable for singular searches, such as searching historic tweets, reading user profile information, or posting Tweets. The Streaming API only sends out real-time tweets, while the Search API (one of the popular REST APIs) gives historical tweets up to about a week with a max of a couple of hundreds. You may request elevated access (e.g. Firehose, Retweet, Link, Birddog or Shadow) for more data by contacting Twitter’s API support.
Basic Uses of Streaming APIs

Create a file called twitter_streaming.py, and copy the code below into it. Make sure to enter your credentials obtained in the Step 1 above into ACCESS_TOKEN, ACCESS_SECRET, CONSUMER_KEY, and CONSUMER_SECRET.




If you run the program by typing in the command:

$ python twitter_streaming.py

You will see tweets keep flowing in your screen. They are a sample of public data (including tweets and also events) flowing though Twitter at the moment. The data returned is in JSON format. It may looks too much for now; it will become clearer in the next step how to read and process this data. Below is one example tweet:


