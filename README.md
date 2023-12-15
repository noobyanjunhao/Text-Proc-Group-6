# Text-Proc-Group-6
Stock News Analysis README

Overview

The StockNews.ipynb Jupyter notebook contains Python code for analyzing news texts in relation to stock prices. It focuses on identifying and visualizing the frequency of certain key words (like names of major tech companies) in news articles over time, and how these frequencies correlate with stock market data.

Contents

StockNews.ipynb: Jupyter notebook containing the Python code for analysis.
Requirements

Python 3.x
Libraries: pandas, matplotlib, csv, collections, datetime
Additional Data: The notebook expects a CSV file named news_stock_price.csv containing news texts along with corresponding dates and possibly stock prices.
Setup and Installation

Ensure Python 3.x is installed on your machine.
Install required Python libraries. This can be done via pip:
Copy code
pip install pandas matplotlib spacy
Clone or download this repository to your local machine.
Running the Code

Place your news_stock_price.csv file in the same directory as the StockNews.ipynb notebook.
Open the StockNews.ipynb notebook using Jupyter Notebook or JupyterLab.
Run each cell in the notebook in sequence. The notebook is divided into sections for easy navigation:
Data Loading and Preprocessing: Reads the CSV file and prepares the data.
Entity Analysis with Spacy: Extracts and analyzes entities from the news texts.
Word Frequency Analysis: Counts the frequencies of specified target words over time.
Data Visualization: Generates and displays plots showing trends in word frequencies.
Output

Upon successful execution, the notebook will display:

A list of the most common entities found in the news text.
Time-series plots showing the trends in word frequencies over time.
