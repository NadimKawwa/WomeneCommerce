# Project: Women's eCommerce

## Downloading the Data

This is a Women’s Clothing E-Commerce dataset revolving around the reviews written by customers. Its nine supportive features offer a great environment to parse out the text through its multiple dimensions. Because this is real commercial data, it has been anonymized, and references to the company in the review text and body have been replaced with “retailer”. The dataset is found on [kaggle.com](https://www.kaggle.com/nicapotato/womens-ecommerce-clothing-reviews/home). The bullet list below explains the features as given by kaggle.

**Features**

1) `Clothing ID`: Integer Categorical variable that refers to the specific piece being reviewed.
2) `Age`: Positive Integer variable of the reviewers age.
3) `Title`: String variable for the title of the review.
4) `Review` Text: String variable for the review body.
5) `Rating`: Positive Ordinal Integer variable for the product score granted by the customer from 1 Worst, to 5 Best.
6) `Recommended IND`: Binary variable stating where the customer recommends the product where 1 is recommended, 0 is not recommended.
Positive Feedback Count: Positive Integer documenting the number of other customers who found this review positive.
7) `Division Name`: Categorical name of the product high level division.
8) `Department Name`: Categorical name of the product department name.
9) `Class Name`: Categorical name of the product class name.


## Libraries

This project requires **Python 3.6** or more recent and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [seaborn](https://seaborn.pydata.org)
- [wordcloud](https://github.com/amueller/word_cloud)
- [os](https://docs.python.org/2/library/os.html)
- [re](https://docs.python.org/2/library/re.html?highlight=re#module-re)
- [bokeh](https://bokeh.pydata.org/en/latest/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. Make sure that you select the Python 2.7 installer and not the Python 3.x installer.


## Motivation

Any organization looking to do business on the internet is interested in what its customers have to say. We want to know if we can predict rating based on the content of the review using natural language processing. We also wan to see if we can predict how likely a customer will recommend products to their friends.


## Summary

First let's look at what people are saying most commnly. The picture below shows a word cloud made from the most common words.
We can see words like fabric, dress, and flattering show up.

![word_cloud](https://github.com/NadimKawwa/WomeneCommerce/blob/master/plots/wordcloud_1.png)

Let's also take a closer look at the age distribution of our clients in the histogram below. Most of the clients are in their late 20s-30s, the distribution appears to be  skewed to an audience of young professionals.

![histo_age](https://github.com/NadimKawwa/WomeneCommerce/blob/master/plots/age_histo.png)

Investigating the data, it comes as no surprise that the relationship between review score and sentiment is positive. That is to say, the more positive a review the higher the score. 

![review_sentiment](https://github.com/NadimKawwa/WomeneCommerce/blob/master/plots/review_vs_score.png)

Finally we wanted to see how likely a customer is to recommend a product. The business relies on a positive experience and in order to grow its products must be recommendation worthy. For this task we build a neural net and predict with 80% accuracy.

We turn our attention to the correlation between the words. The plot below shows the t-distributed Stochastic Neighbor Embedding for the most polarized words. The idea is to cluser together words that have the nearest 'feeling'.

![tsne_1](https://github.com/NadimKawwa/WomeneCommerce/blob/master/plots/bokeh_plot.png)

In order to see more clearly what is happening, we zoom in on two regions. The plots below show a clearer view. We can see 'lovely', 'comfy', and 'better' lumped together. Conversly, negative words such as 'cheap' and 'returning' are grouped together.

![tsne_2](https://github.com/NadimKawwa/WomeneCommerce/blob/master/plots/bokeh_plot-2.png)

![tsne_3](https://github.com/NadimKawwa/WomeneCommerce/blob/master/plots/bokeh_plot-3.png)
