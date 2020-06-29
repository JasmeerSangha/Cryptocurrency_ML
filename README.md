# Cryptocurrency_ML

## Resources
- Data: [Cryptocurrency data](https://github.com/JasmeerSangha/Cryptocurrency_ML/blob/master/Data/crypto_data.csv)
- Tools: Python 3 scikit library

## Analytical Process
- Extract and tranform the data.
- Reduce data to 3 dimensions using PCA.
- Cluster data using K-means
- An elbow curve was created to choose K value
- The model was fit and used to group data into classes
- Visualize results using Plotly Express and hvplot

## Summary
After transforming the data and recuding the columns to three principle components, the elbow curve suggests there are 4 distinct clusters within the data:
![](https://github.com/JasmeerSangha/Cryptocurrency_ML/blob/master/Images/elbow_plot.png)
The following 3D plot shows there is a single point, BitTorrent, in cluster 2. Clusters 0 and 3 share PC1 and PC3 vaues near zero(0) and only differ in the sign of their PC2 values. Cluster 1 is the only group with PC3 > 5:
![](https://github.com/JasmeerSangha/Cryptocurrency_ML/blob/master/Images/3D_PCA.png)
Finally, I have created a plot comparing coins mined to the total coin supply. This view make sit difficult to dicern any differnce between clusters 0,1,3. Again BitTorrent, the oultier, is seperated form the rest of the group as its coins mined and supply limit, far exceed the others. 
![](https://github.com/JasmeerSangha/Cryptocurrency_ML/blob/master/Images/MinedvsSupply.png)
