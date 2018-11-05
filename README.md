# HN_Search

This is the repository regarding the analysis of the Hackernews search query dataset.

This analysis is done in Python, in an interactive way through Jupyter notebooks.

The required packages for this analysis are in the file requirements.txt
I would advise to create a dedicated virtualenv in order to not mess with you current python installation.

The visualisation in the notebooks are done through the plotly visualisation library, and is highly recommended due to it's interractivity.
However, because of the number of datapoints the visualtion are several megabytes, the images we be cleared from the notebooks, and it's recommanded to run the notebooks.
A static version of the images will be in the folder images/


3 notebooks are provided in this analysis: 

- EDA.ipynb: This notebook is the first to open, as it acts as an exploratory notebook around the dataset, and the findings in this notebooks will lead to the other two.
  
- Clustering.ipynb: This notebook is the reflexion of the study on how can we cluster user search queries in an unsupervised manner, in order to better provide insights on the type of queries.
  
- Trends_per_day.ipynb : This notebook is used as a study on how can we compute, in an efficient manner, trending queries per day, in order to have a better representation of what queries are done in an time interractive manner.

The notebooks are using a concatenated version of the dataset
The notebooks are using fasttext wordvectors, trained on the CommonCrawl Dataset, available at this [address](http://fasttext.cc)
