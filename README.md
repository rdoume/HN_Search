# HN_Search

This is the repository regarding the analysis of the Hackernews search query dataset.


## Requirements

This analysis is done in Python, in an interactive way through Jupyter notebooks.

The required packages for this analysis are in the file requirements.txt

FastText can be tricky to install, you should follow the instructions on their [github](https://github.com/facebookresearch/fastText#building-fasttext)

I would advise to create a dedicated virtualenv in order to not mess with you current python installation.
These notebooks have been tested under Ubuntu 16.04 and Mint Sonia

## External data

The notebooks are using  the binarized fasttext wordvectors, trained on the CommonCrawl Dataset, available at this [address](https://s3-us-west-1.amazonaws.com/fasttext-vectors/crawl-300d-2M-subword.zip)
One you downloaded the wordvectors, you shall put in the the data folder.


## Prepare the dataset

The data has been given as separate day data.
For the sake of simplicity, I concatenated each file as a unique one with the command 

```bash

cat ./data/2018* > all.txt

```

This file all.txt is required in order

## Visualisation

The visualisation in the notebooks are done through the plotly visualisation library, and is highly recommended due to it's interractivity.

However, because of the number of datapoints the visualtion are several megabytes,the notebook will contains static version of the visualisation, therefore, you should re-run the notebooks

A static version of the images will be in the folder images/

3 notebooks are provided in this analysis:

- EDA.ipynb: This notebook is the first to open, as it acts as an exploratory notebook around the dataset, and the findings in this notebooks will lead to the other two.
  
- Clustering.ipynb: This notebook is the reflexion of the study on how can we cluster user search queries in an unsupervised manner, in order to better provide insights on the type of queries.
  
- Trends_per_day.ipynb : This notebook is used as a study on how can we compute, in an efficient manner, trending queries per day, in order to have a better representation of what queries are done in an time interractive manner.
