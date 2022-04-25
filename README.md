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

Register for Reddit API here: https://www.reddit.com/wiki/api . Then type in your keys

```python
CLIENT_ID = ''
SECRET_KEY = ''
```

Subreddit

```python
#single subreddit
sub = 'SustainableFashion'
#use plus sign to combine subreddit
sub = 'SustainableFashion+python'
#use all for all subreddit 
sub = 'all'
```

Keyword, sort , and time_filter

```python
#the keyword is limited to a single string
keyword='brand'
# sort – Can be one of: relevance, hot, top, new, comments. (default: relevance).
# time_filter – Can be one of: all, day, hour, month, week, year (default: all).
sort =''
time_filter =''
```

## Section 3

Create a csv file for each submission

```python
all = reddit.subreddit(sub)

#limit maxinum is 1000
for submission in all.search(keyword, sort, time_filter, limit= 2):
```



## Variables

| title                    | title of the submission                                     |
| :----------------------- | ----------------------------------------------------------- |
| Variable name            | Description                                                 |
| author                   | author of the submission                                    |
| author_des               | author bio (mostly mull)                                    |
| comment                  | comment replied to the submission                           |
| comment_author           | comment author (could be null)                              |
| comment_author_des       | comment author bio(mostly null)                             |
| comment_reply            | reply to the comment (not directly reply to the submission) |
| comment_reply_author     | reply author (could be null)                                |
| comment_reply_author_des | reply author bio (mostly null)                              |

