# Unlocking Financial Innovation: A Paradigm Shift in Cryptocurrency Portfolio Construction through Unsupervised Learning 
## Executive Summary:
In response to the evolving landscape of cryptocurrency investment, this project proposes a novel approach to assembling investment portfolios based on cryptocurrencies. Traditionally, portfolio construction relies heavily on metrics such as returns and volatility. However, this project introduces a multifaceted methodology incorporating additional factors impacting the crypto market to enhance portfolio performance. Leveraging financial Python programming skills and unsupervised learning techniques, specifically K-means clustering and principal component analysis (PCA), presenting a prototype for constructing crypto portfolios. The methodology involves clustering cryptocurrencies based on their performance over different periods and visualizing the results to facilitate decision-making for the board of directors of a business entity.
## Methodology:
- Data Preparation: The cryptocurrency price change data provided in the CSV file was imported and prepared.
- Finding the Best Value for k (Original Data): Using the original data, the elbow method algorithm was implemented to determine the optimal value for k (number of clusters). A line chart of inertia values for different values of k was plotted, and the best value was identified.
- Cluster Cryptocurrencies with K-Means (Original Data):
  - A K-means model was initialized with the best value for k.
  - The model was fitted with the original data, and clusters were predicted.
  - A scatter plot was created using hvPlot to visualize the clusters.
- Optimizing Clusters with PCA:
  - A PCA model instance was created, and features were reduced to three principal components.
  - The explained variance was assessed to understand the contribution of each principal component.
  - A new DataFrame with PCA data was created, retaining the coin_id index from the original DataFrame.
- Finding the Best Value for k (PCA Data): The elbow method was applied using PCA data to find the optimal value for k. Inertia values were plotted and compared with results from the original data.
Cluster Cryptocurrencies with K-Means (PCA Data):
  - A K-means model was initialized with the best value for k obtained from PCA data.
  - The model was fitted with PCA data, and clusters were predicted.
  - Clusters were visualized using a hvPlot scatter plot.
 
