# Crypto Clustering

In this challenge, we focus on unsupervised machine learning. Specifically, we use the k-means clustering and principal component analysis to reduce features.

## Goal

For this challenge, we were provided with some data for various crypto currencies. Following are the steps we performed for the analysis:
1. Imported the data from a csv to a dataframe and scaled it using the "StandardScalar" function.
2. Then we created a elbow curve (inertia plot) using k-means clustering method to find the best value of *k* on this original scaled data.
3. Fitted the original scaled data for k-means clustering using the ideal *k* value (k = 4) found in the previous step. We then plotted the first two features and highlighted the predicted clusters.
4. In this next part, we used principal component analysis (PCA) method to reduce the dimensions/features. We fitted the scaled data using the PCA function and setting the number of compenents as 3. We also found the total explained variance (= 0.8950316570309842) by these 3 components.
5. Then we repeated step 2 to find the ideal *k* value and the result was again k = 4.
6. Using k = 4 and the new PCA data, we repeated step 3 and performed k-means clustering. We again plotted this data using the first two components.
7. Finally, we compared the results of elbow curves and cluster plots from using the original scaled data vs the PCA data and found the number of clusters were preserved.
