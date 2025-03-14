# CryptoClustering

This repository contains the code for the CryptoClustering project, where the goal is to apply unsupervised learning techniques (K-Means clustering and PCA) to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

The project involves data preprocessing, feature scaling, clustering, and optimization using principal component analysis (PCA).

## Before You Begin
1. Create a new repository named CryptoClustering and clone it to your local machine.
2. Push your changes to GitHub once you're ready.
## Files to Download:
* Module 19 Challenge files: Make sure you download and set up the starter code as outlined in the instructions.
  
## Project Steps
1. Load and explore data:

* Load the crypto_market_data.csv into a pandas DataFrame.
* Analyze the summary statistics and plot the data.

2. Prepare Data:

* Normalize the data using StandardScaler() from scikit-learn.
* Set the "coin_id" index from the original DataFrame.

3. Find the Best Value for k Using the Scaled DataFrame:

* Use the elbow method to determine the optimal value for k.
* Plot the elbow curve to visualize the inertia values.

4. Cluster Cryptocurrencies with K-means:

* Apply K-means clustering with the optimal value for k.
* Visualize clusters using hvPlot.

5. Optimize Clusters with Principal Component Analysis (PCA):

* Perform PCA to reduce the features to three components.
* Compute the explained variance for each component.
* Create a new DataFrame with the scaled PCA data.

6. Find the Best k Value Using the PCA DataFrame:

* Apply the elbow method on the scaled PCA data and determine the optimal k.
* Compare it with the k value from the original scaled data.

7. Cluster with K-means using PCA Data:

* Perform K-means clustering on the PCA data.
* Visualize the results in a scatter plot.

8. Visualize and Compare the Results:

* Create composite plots using hvPlot to compare the elbow curves and clustering results from both the original scaled DataFrame and the scaled PCA DataFrame.
  
## Requirements
To run this project, you'll need Python 3.x and the following dependencies:

* pandas
* scikit-learn
* hvplot
* matplotlib
