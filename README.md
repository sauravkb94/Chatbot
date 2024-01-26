# Chatbot ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/NLTK)

![GitHub Repo stars](https://img.shields.io/github/stars/sauravkb94/Chatbot) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eobwBwanstVKYHJ_c4KA6SEWQHeLLC1f#scrollTo=WWROT7gyJ2fN)

<img src="https://github.com/sauravkb94/Chatbot/blob/main/chat-bot.png" align="left"
     alt="Chatbot" width="90" height="90">
## A chatbot that responds to a specific text that you provide using nltk lib (NLP) and  Cosine similarity for similarity score and builds a basic application


**nlp_utils**- nltk stand for natural lang toolkit used for building python prohrams which work with human lang data and natural language processing.
**string**- is concatenation of ASCII Lowercase and ASCII uppercase string constant
**pandas**- python lib used to create data frames and help us to manipulate these data frames (read, load and manipulate the dataset.
**matplotlib.pyplot** -is a collection of functions that make matplotlib work like MATLAB. Each pyplot function makes some change to a figure: e.g., creates a figure, creates a plotting area in a figure, plots some lines in a plotting area, decorates the plot with labels, etc.


In this, I have divided the dataset into Query and Response using Panda function

1. ***Data visualization***

- I used sentiment analysis (to verify the repetition and if the statement  is positive, negative or natural) - **import SentimentIntensityAnalyzer**, it does have a dictionary which already assigned values for corresponding. **from nltk.sentiment.vader**  NLTK Vader sentiment analyzer is a rule-based model for sentiment analysis of social media text. It is a part of the Natural Language Toolkit (NLTK), which is a popular Python library for working with human language data. The Vader model uses a lexicon of words and their sentiment scores to determine the sentiment of a given text. It also takes into account punctuation, capitalization, and intensifiers to provide a more accurate sentiment score. The Vader model is particularly useful for analyzing short texts such as tweets, reviews, and comments.
> Example : - why would i do that? - neg: 0.0, neu: 1.0, pos: 0.0, compound: 0.0,
- **import WordCloud**, A word cloud is a visual representation of the most frequently used words in a text. The words are arranged in a way that the more frequently a word appears in the text, the larger and more prominent it appears in the word cloud 

2. ***Text Normalization***
- we change our text and convert the text into a usable form, where we remove all the specail chars and we convert the text in lowercase, also remove any non ASCII characters and alphanumeric values as well. help us to covert in upper to lower,number into words, remove white space, expand abbreviation and also we can remove words(most fequently words).**import re**  regular expressions

Import **tfidf** victimizer will fit_transform takes to feature vectors, which can be used as an input to estimate.So it converts each token or a word to a feature index in the matrix where each unique token gets a feature index.Then we have changed it to an array 
once we had converted our query column into TFIDF. I have used **cosine_distance**(To measure the similarity, it is one of the most widely used and powerful similarity measures in data science, and it is used in the cases of NLP or natural language processing used for information retrieval. It is also used in multiple applications).


