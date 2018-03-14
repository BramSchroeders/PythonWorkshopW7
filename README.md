# Workshop Python 14/03

The main goal of this workshop is to familiarise yourself with Python and some of the most important modules it has to provide.
It's not important to gain a deep understanding in these modules, raising awareness of their existance and capabilities is key.


## Working environment and preliminaries

To achieve this goal, you will use Spyder. Spyder is an IDE for Python development. Open Spyder by pressing <kbd>⊞ Win</kbd> and typing 'Spyder'. Spyder's user interface is straightforward, the instructor will help you get started.

## The beer data set
The dataset we will be using in this workshop is the beer data set. The description of this data is can be found [here](https://www.kaggle.com/c/beer-ratings/data "The beer data set").

## Access the data
[Pandas](https://pandas.pydata.org/ "Pandas website") is a data analysis module for Python. One of the features is accessing data.
Import pandas by using:
```python
import pandas as pd #as pd is optional but it's more practical to use aliases
```
Now use Pandas to read the CSV file in a [DataFrame](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.html).
<details><summary><b>Hint</b></summary>
<p>
  
```python
beer_data = pd.read_csv('path_to_your_csv_file.csv')
```

</p>
</details>


### Basic statistics

Use the Pandas library to do the following tasks:
* Calculate the mean, standard deviation, and variance of the ABV
* What's the name of the beer with the highest ABV?
* What's the name of the beer with the lowest ABV?
* What's the mean, standard deviation, and variance of  the scores?
* How many styles of beer are represented? Write a list of all types to CSV file.
* What's the average score and ABV for each beer style? What's the top 5?

### Processing reviews and Score prediction

## POS-tagging
Part-of-speech tagging (POS-tagging) is the process of identifying parts of senteces and tag them. An example using NLTK can be found [here](http://www.nltk.org/book/ch05.html).

* Use nltk to POS tag some reviews. This is relatively computational expensive so limit it to the first 100 reviews.
* Filter the adjectives out of your POS-tagged sentences since they describe your beer. What's the top 5 most used adjectives?

## Sentiment Analysis
Sentiment analysis is automatically detecting the sentiment of a person, usually in writing. Different systems exist, but the sentiment is oftenly quantified as a number between -1 (negative) and 1 (positive) with 0 being neutral.

* Use the requests library to perform a [this](http://text-processing.com/docs/sentiment.html) sentiment API. Limit yourself to 5 requests since the number of requests per day is limited.
* Use VADER in nltk to perform sentiment analysis on your reviews. An example can be found [here](http://www.nltk.org/howto/sentiment.html). Add sentiment to the dataframe.


