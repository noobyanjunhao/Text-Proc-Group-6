# Text-Proc-Group-6
Stock News Analysis README

## Overview

The StockNews.ipynb Jupyter notebook contains Python code for analyzing news texts in relation to stock prices. It focuses on identifying and visualizing the frequency of certain key words (like names of major tech companies) in news articles over time, and how these frequencies correlate with stock market data.

## Contents

StockNews.ipynb: Jupyter notebook containing the Python code for analysis.
The code begins with the **first cell**, which first uses csvreader to read in our file. We create a list (ft_rows) of all the cells in column 3 which contains the full text of the news articles we are analyzing. We then customize and tokenize the text to create bigrams. 
**Cell two** deals with finding statistics about our data like total words, total tokens, and average sentences per report.
**Cell three** just prints out the first 500 tokens which we were just using for data exploration.
**Cell four** prints the top 50 tokens and their frequencies.
**Cell five** deals with creating bigrams for the normalized text.
**Cell six** makes a word cloud for the full text. The text is lemmatized before being converted to wordcloud. 
**Cell seven** filters the dataset so only rows where a specific word is mentioned is included in the new list. We used this to analyze different large tech companies like Apple, Tesla, and Microsoft. 
**Cell eight** tokenizes the text with the filtered rows the same way as before. 
**Cell nine** deals with finding collocations using pmi score and a filter of 10. 
**Cell ten** uses pandas to create a dataframe.
**Cell eleven** uses spaCy to find common entities
**Cell twelve** uses plt to plot the frequencies of the different entities



## Python 3.x
Libraries: pandas, matplotlib, csv, collections, datetime

## Setup and Installation
Ensure Python 3.x is installed on your machine.
Install required Python libraries. This can be done via pip:
Copy code
pip install pandas matplotlib spacy

Place your news_stock_price.csv file in the same directory as the StockNews.ipynb notebook.
Open the StockNews.ipynb notebook using Jupyter Notebook or JupyterLab.
Run each cell in the notebook in sequence. The notebook is divided into sections for easy navigation:
Data Loading and Preprocessing: Reads the CSV file and prepares the data.
Entity Analysis with Spacy: Extracts and analyzes entities from the news texts.
Word Frequency Analysis: Counts the frequencies of specified target words over time.
Data Visualization: Generates and displays plots showing trends in word frequencies.
Output

## Output:
Top bigrams
Top Collocations
A list of the most common entities found in the news text.
Time-series plots showing the trends in word frequencies over time.
