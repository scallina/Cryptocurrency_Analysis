# Cryptocurrency_Analysis

## Overview

In this analysis, I created utilized Unsupervized Machine Learning to analyze what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for new investments.

Since there was no specific output for the dataset I was working with, I utilized unsupervised learning - specifically a clustering algorithm. 

## Approach

### First, I used Pandas to clean the dataset, which was retrieved from  CryptoCompare (https://min-api.cryptocompare.com/data/all/coinlist). 
- I filtered the data to only show coins that were currently trading and that have been mined. 
- I used get_dummies() to encode my text features
- I utilized a standard scaler to standardize my features across the datframe. 

### Second, I utilized Principal Component Analysis (PCA) to reduce my dimensions to 3 principal components. 
- I placed these principal components into a new dataframe, which would be merged with the main set later. 

### Third, I used a K_means algorithm to predict clusters for my dataset. 
- I utilized an hvplot elbow curve to determine the best K-value. I decided to use 4 clusters after examining the elbvow curve. 

## Results

### I utilized plotly and hvplots to create visualizations demonstrating the clustering of the various cryptocurrencies I analyzed in this project. This analysis should be helpful for thos interested in investing in crypto and looking to diversify their portfolio across various investment types. 
