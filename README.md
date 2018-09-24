# Content: Natural Language Processing
## Project: Women's eCommerce

### Install

This project requires **Python 2.7** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [seaborn](https://seaborn.pydata.org)
- [wordcloud](https://github.com/amueller/word_cloud)
- [os](https://docs.python.org/2/library/os.html)
- [re](https://docs.python.org/2/library/re.html?highlight=re#module-re)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. Make sure that you select the Python 2.7 installer and not the Python 3.x installer.

### Code

Template code is provided in the `Women_Ecommerce.ipynb` notebook file. You will also be required to use  the `Womens Clothing E-Commerce Reviews.csv` dataset file to complete your work.
### Run

In a terminal or command window, navigate to the top-level project directory `customer_segments/` (that contains this README) and run one of the following commands:

```bash
ipython notebook Women_Ecommerce.ipynb
```  
or
```bash
jupyter notebook Women_Ecommerce.ipynb
```

This will open the Jupyter Notebook software and project file in your browser.

## Data

This is a Women’s Clothing E-Commerce dataset revolving around the reviews written by customers. Its nine supportive features offer a great environment to parse out the text through its multiple dimensions. Because this is real commercial data, it has been anonymized, and references to the company in the review text and body have been replaced with “retailer”. The dataset is found on [kaggle.com](https://www.kaggle.com/nicapotato/womens-ecommerce-clothing-reviews/home).

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
