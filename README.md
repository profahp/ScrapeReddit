# ScrapeReddit

This code is design for you to scrape user's profile in a subreddit. 

Use git clone to download the code. 

git clone https://github.com/shinyshwn/ScrapeReddit.git

## Section 1

Install all the packages. If you run into any missing packages running the program, you can use this format to install packages import it. 

```pyth
!pip install package
import package
```

## Section 2

Register for Reddit API here: https://www.reddit.com/wiki/api . Then type in your keys and account password

```py
CLIENT_ID = ''
SECRET_KEY = ''
# username and password 
data = {
    'grant_type': 'password', 
    'username': '', 
    'password': ''
}
```

## Section 3

Get a list of users names in the subreddit you interested in. 



## Section 4

Scrape the user profile into csv files. There are two csv files for each user, one for comments and one for their submissions.
