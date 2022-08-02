# Cryptocurrencies
In this analysis I processed data, reduced dimensions, used K-means to cluster, and then created visualizations that would help decide if we can trade a specific crypto currency or not.

## OverView
A prominent investment bank is interested in offering a new cryptocurrencies investment portfolio for its customers, however, they are lost in the immense universe of cryptocurrencies. They ask you to help them make sense of it all by generating a report of what cryptocurrencies are available on the trading market and how they can be grouped using classification. They’ve asked you to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

## Summary
Prepare data for dimension reduction with PCA and clustering using K-Means. We've also reduced data dimensions using PCA and the completion of this task results in the df_crypto_scaled_pca dataframe:

Then we've clustered cryptocurrencies using K-Means; first creating an Elbow Curve to find the best value for k. Once we've determined the k value we thought best fits, we've used the k-means clustering algorithm to the predict the k clusters for the processed data. Results are:

![image](https://user-images.githubusercontent.com/95777297/182272272-259a8b30-5b11-4d08-83d2-42159c2e0ae6.png)

## Analysis
- A 3D-Scatter using hvPlot to plot the clusters.
- Using hvplot.table to create a data table with all the current tradable cryptocurrencies.
- Create a scatter plot using hvplot.scatter, to present the clustered data about cryptocurrencies having x="TotalCoinsMined" and y="TotalCoinSupply" to contrast the number of available coins versus the total number of mined coins.
 
 ![image](https://user-images.githubusercontent.com/95777297/182272455-43aa876a-7e35-44dd-ac99-df37ac53e1ad.png)
