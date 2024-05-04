# CerealClustering

## Objective
Utilize an unsupervised machine learning model in Python to create clusters in a cereal dataset.

## Data Source
- [80 Cereals](https://www.kaggle.com/datasets/crawford/80-cereals/data) from Kaggle

## Methods
1. Read in the CSV cereals file
2. Preprocess the data by:
   - Removing vitamins, shelf, weight, cups, and rating columns - these columns felt irrelevant to the dataset
   - Applying standard scaler to numerical data
   - Encoding the categorical data (manufacturer and type)
3. Employ an elbow curve to determine the ideal number of clusters for the data
4. Initiate a kmeans model with 5 clusters and create predictions for the data
5. Graph the initial predictions comparing calories to sugar content
6. Create a PCA model with two components
7. Fit the dataset to the PCA model (which explained 52% of the variance)
8. Execute an additional elbow curve with the PCA data (4 clusters)
9. Initiate a kmeans model with the PCA data
10. Graph the new PCA predictions comparing the two PCA components


## Results
- The initial dataset before applying kmeans did not result in clear clusters. After applying PCA, 4 prominent clusters were visible once graphed.

## Figures
![image](https://github.com/lvit001/CerealClustering/assets/140283164/acbfa06d-2439-4476-959e-c90face8913c)
- Elbow curve with initial data, elbow at 5

![image](https://github.com/lvit001/CerealClustering/assets/140283164/b55a07b2-1a84-400c-85a7-c2f601c73941)
- Scatterplot with initial dataset comparing calories to sugar, 5 clusters

![image](https://github.com/lvit001/CerealClustering/assets/140283164/433c9ff6-d5df-440e-bb30-b1397bbc2bcd)
- Elbow curve with PCA dataset

![image](https://github.com/lvit001/CerealClustering/assets/140283164/7d5ec868-1e63-4cd8-9af8-efb84d5c9ae8)
- Scatterplot with PCA data, 4 clear clusters

