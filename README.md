# Cryptocurrency-Clusters

This project consisted of building unsupervised machine learning models to explore whether cryptocurrencies can be grouped together with other similar cryptocurrencies.

![Crypto Compare Logo](Images/CryptoCompareLogo.jpg)

## Background

The vast universe of cryptocurrencies can be overwhelming. To tackle the vastness, unserpervised machine learning models were used to create a a report that includes what cryptocurrencies are on the trading market and determine whether they can be grouped to create a classification system for this new investment.

Raw data from [Crypto Compare](https://www.cryptocompare.com/) was used to fit the machine learning models. Since there is no known classification system within the data, unsupervised machine learning models were chosen. 

## Data Preparation

A [dataset]https://min-api.cryptocompare.com/data/all/coinlist) from Crpto Compare was initially read that included information for each cryptocurrency.

Data preparation is then processed so that the raw data will fit the unsupervised machine learning models.

## Dimensionality Reduction

Once data preparation took place, dimentionality reduction was performed with PCA. Using PCA, 90% of the explained variance in dimensionality reduction was preserved.

Further reduction took place afterwards using t-SNE on the principal components: the output of the PCA transformation. A scatter plot was then created using the t-SNE output to observe whether there are distinct clusters or not.

## Cluster Analysis with k-Means

The final step in this project included creating an elbow plot to identify the best number of clusters. A for-loop was used to accomplish this step. 

## Overall Considerations

Based upon the findings uncovered while working through this project, cryptocurrencies can be clustered together. 

The number of clusters can be determined by looking at the elbow curve. By observing the elbow curve, it can be determined that cryptocurrencies can be clustered into 4 groups. 