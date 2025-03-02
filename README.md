# CryptoClustering
By: Itzel Vázquez Sánchez

## Project Description

This project is part of the Data Analysis and Visualization Bootcamp from Tecnológico de Monterrey. In this assignment, the task was to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

### Prepare the Data:
1. Use the StandardScaler() module from scikit-learn to normalize the data from the CSV file.
2. Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame. The first five rows of the scaled DataFrame should appear as follows:
   ![image](https://github.com/user-attachments/assets/b178c987-02e1-4dfd-9af5-46f08906155c)


### Find the Best Value for k Using the Scaled DataFrame
3. Use the elbow method to find the best value for k.
4. Answer the following question in your notebook: What is the best value for k?

### Cluster Cryptocurrencies with K-means Using the Scaled DataFrame
5. Cluster the cryptocurrencies for the best value for k on the scaled DataFrame.
6. Create a scatter plot using hvPlot. Set the x-axis as "price_change_percentage_24h" and the y-axis as "price_change_percentage_7d". Color the graph points with the labels found using K-means. Add the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data point.

### Optimize Clusters with Principal Component Analysis
7. Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components.
8. Retrieve the explained variance to determine how much information can be attributed to each principal component and then answer the following question in your notebook: What is the total explained variance of the three principal components?
9. Create a new DataFrame with the scaled PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame. The first five rows of the scaled PCA DataFrame should appear as follows:
  ![image](https://github.com/user-attachments/assets/0a035954-4b8b-4d45-8eb3-97454fac45ca)

### Find the Best Value for k Using the PCA DataFrame
10. Use the elbow method on the scaled PCA DataFrame to find the best value for k.
11. Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.
12. Answer the following questions in your notebook: What is the best value for k when using the scaled PCA DataFrame? Does it differ from the best k value found using the original scaled DataFrame?

### Cluster Cryptocurrencies with K-means Using the PCA DataFrame
13. Cluster the cryptocurrencies for the best value for k on the PCA DataFrame. 
14. Create a scatter plot using hvPlot as follows: Set the x-axis as "PC1" and the y-axis as "PC2". Color the graph points with the labels found using K-means. Add the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data point.
15. Answer the following question: What is the impact of using fewer features to cluster the data using K-Means?

### Composite plots
16. Create composite plots by using hvPlot to compare the elbow curve that you created from the original scaled DataFrame with the one that you created from the scaled PCA DataFrame.
17. Create a composite plot by using hvPlot to compare the cryptocurrency clusters that resulted from using the original scaled DataFrame with those that resulted from the scaled PCA DataFrame.
18. Answer the following question: Based on visually analyzing the cluster analysis results, what's the impact of using fewer features to cluster the data by using K-means? 

🤓 This Project is the result of the learning lessons of Module 19: Unsupervised Learning from the Data Analysis and Visualization Bootcamp 2024. The main goal is to use the acquired habilities and knowledge in a real case. 

## Table of contents :point_right:

On the repository you'll find:

| Item | File Type|   File Name             |   Description                      |
|------|----------|-------------------------| -----------------------------------|
|1     | folder   | Resources/.csv          |Contains crypto_market_data.csv file|
| 2    |  ipynb   | Crypto_Clustering.ipynb | From starter code                  |


## How to Use the Project

* First, clone or download the repository so you have the csv on the Resources folder.
* The Crypto_Clustering.ipynb file contains the code to the answers of the challenge. You can run it in Jupyter Notebook or in Visual Studio Code.

## Credits :scroll:
The code of this project origins from: starter code provided by the Team of the Data Analysis and Visualization Bootcamp, the solved exercises worked in the Zoom Lessons, Holoviz [Documentation](https://holoviz.org/tutorial/Composing_Plots.html) and Microsoft Copilot.
