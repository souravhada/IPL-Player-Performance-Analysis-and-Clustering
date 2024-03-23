# IPL Player Auction Price Prediction

## Overview
This repository contains a dataset consisting of information on 90 IPL players. The business case we are considering involves grouping the players to set a suitable base price for the upcoming auction. We utilize K-means clustering for this purpose.

## Methodology
We performed the following steps:
1. **Exploratory Data Analysis (EDA):** 
   - Removed null values.
   - Conducted `df.info()` and `df.describe()` to understand the dataset.
   - Plotted graphs for top 10 players with the highest run, average, and strike rate.
   - Utilized distplot, box plot, and correlation heatmap for further analysis.

2. **K-means Clustering:**
   - Utilized the elbow method and Within-Cluster Sum of Squares (WSS) to determine the optimal number of clusters.
   - Achieved the best fit with 2 clusters, supported by a silhouette score of approximately 0.411.
   
3. **Cluster Analysis:**
   - Cluster 1 (Class 1): Consisted of 35 players.
     - Players in this cluster exhibited higher statistical performance, with a mean total score of around 372.
     - Other features such as average, strike rate, number of fours and sixes, and number of half-centuries were significantly higher compared to Cluster 2.
     - These players were labeled as Grade A players.
   
   - Cluster 2 (Class 0): Consisted of 55 players.
     - Players in this cluster had comparatively lower statistical performance, with a mean total score just above 120.
     - Labeled as Grade B players.
     
   - Note: This analysis specifically pertains to batting stats and does not include bowling or fielding.

## Conclusion
Through K-means clustering, we successfully categorized IPL players into two distinct groups, Grade A and Grade B, based on their batting performance. 
For more details, refer to the Jupyter notebook provided in this repository. 

**Author:** Sourav Singh Hada

