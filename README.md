# crypto_evaluator

Purpose: The purpose of this project is to utilize Unsupervised Machine Learning that seeks to draw comparisons and correlations between over 1100 cryptocurrencies.  In this project, I utilized data from CryptoCompare to filter for mined currencies in order to determine if these coins can be grouped to create a visualization for potential crypto investor.  

Utilized the following:
- Python
- Pandas Notesbook
- SKLEARN Models: Standard Scaler, PCA, T-SNE, K-Means
- pd.getdummies()


The process:

First, I prepared the data by dropping not quantifiable metrics such as the coin name.  I then used pd.getdummies() to convert the Algorithm and Prooftype columns into a numerical data to create the variables.  In addition, I dropped all coins that had yet to be mined from this dataframe.  

Secondly, I standardized the data using Standard Scaler performed dimensionality reduction reducting with PCA while preserving 90% of the data.  

Thirdly, I utilized the T-SNE model to create a scatter plot to create clusters to discover if the quality of each cryptocurrency is correlated or if there is discrepencies between the utilization of each crypto. 

Lastly, I utilized the K-means model to find the ideal # of clusters within the crypto data provided.  The K-means model showed that the ideal number of clusters for the filtered and reduced data is 4.  

Conclusion:
This model proves to investors that there are deep discrpencies between the quality of cryptocurrency due to the network and framework behind each crypto.  Some cryptos such as AVAX, Solana, Cardano have a much stronger framework due to the amount of engineers and backing behind it.  This model proves to investors that crypto currencies cannot be lumped into one category and that investors need to be highly selective.  

