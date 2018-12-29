# NHL Team Twiiter Bot

This bot randomly selects 5 of the 31 NHL Teams to source from every time, and generates a tweet with similar sentiment and content using a Markov Chain model. The code is largely based off of [this repository](https://github.com/tommeagher/heroku_ebooks), with a few small modifications. Please see the original repository for a step-by-step guide on setting up Heroku.

## Local setup
- `pip3 install` these packages:
  + `python-twitter`, which I've found to work better than just `twitter`
  + `Mastodon.py`
  + `bs4`
- `touch .env` to create a `.env` file, in this format:
```py
export TWITTER_CONSUMER_KEY='[your consumer key, in quotes]'
export TWITTER_CONSUMER_SECRET='[your consumer secret, in quotes]'
export TWITTER_ACCESS_TOKEN_KEY='[your access token key, in quotes]'
export TWITTER_ACCESS_SECRET='[your access token secret, in quotes]'
```
- `source .env` to add these to your environment
- `python3 ebooks.py` to run the program


## Credit
- [@harrisj](https://twitter.com/harrisj)'s [iron_ebooks](https://github.com/harrisj/iron_ebooks/)

- [Tom Meagher](http://www.tommeagher.com)'s [heroku_ebooks](https://github.com/tommeagher/heroku_ebooks)

- Daniel Peterschmidt's [Medium article](https://medium.com/science-friday-footnotes/how-to-make-a-twitter-bot-in-under-an-hour-259597558acf)
