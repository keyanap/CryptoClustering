# CryptoClustering

In this challenge, I used unsupervised learning to predict if cryptocurriences are affected by 24-hour or 7-day price changes. I started with loading the csv file into a dataframe, and gathered it's summary statistics. I then prepared the data using the StandardScaler module from scikit-learn and used it to normalize the data. Following that, I created a dataframe with the scaled data and set the index as the crypto coin names. 

I then used the elbow method to find the best value for k. To do so I created an empty list to store interia values and created a list of k values from 1 to 11. I created a dictionary with the data needed to plot the elbow curve. I then ploted the line graph for the elbow curve and it revealed that 4 is the best value for k. The K-means model was then initialized with the k value of 4. Predictions were made and placed as a new column in a copy of the scaled dataframe. I created the scatter plot using hvPlot. 


![Alt text](<Screenshot 2024-01-11 at 1.02.04 PM.png>)


I then performed a PCA to reduce the features to three prinicipal componenets. I again created a list for k vlues from 1 to 11 and an empty list to store the inertia values. I created a dictionary to place all the data needed to plot the elboew curve. This found that 4 was the best k-value. The K-means model was then initialized with the k value of 4. Predictions were made and placed as a new column in a copy of the scaled dataframe. I created the scatter plot using hvPlot. 


![Alt text](<Screenshot 2024-01-11 at 1.22.53 PM.png>)


I then created two plots; one that showed both elbow curves and one that showed both scatter plots. 


![Alt text](<Screenshot 2024-01-11 at 1.21.20 PM.png>)


![Alt text](<Screenshot 2024-01-11 at 1.21.22 PM.png>)


