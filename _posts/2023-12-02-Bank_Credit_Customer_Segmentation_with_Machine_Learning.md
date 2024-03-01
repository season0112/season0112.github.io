---
layout: post
comments: true
title: Bank Credit Customer Segmentation with Machine Learning (K-Means and Random Forest)
categories: [Banking Risk Project]
---

<!-- url is: /home/category/year/month/day/XXX.html -->

This is machine learning data project about banking credit risk evaluation. The goal of this project is to help the bank risk team to estimate the risk level for bank credit customers.

Data Source: The data is from a German Bank collected by Porf Hofmann of the University of Califonia in 2016. It contains the 1000 customers information about their ages, jobs, accounts status and banking credit etc. Missing data is filled with "unknown" due to the non-negligible amount.

In Figure 1, the customer credit picture is drawn. Credit amount, duration and purpose are given.

![Customer_Credit_Picture.jpg](../../../../../figure/Customer_Credit_Picture.jpg)
<center>Figure 1: Customer credit amount, duration and purpose. </center>

There are two kinds of customers information: Classified Features and Continued Features. For the Classified Features, tag coding is applied. For the Continued Features, the Standardisation is applied.

To evaluate the credit risk, K-Means Clustering method is used. Here, the number of clustering is set to be 4 which is determined by elbow method. In Figure 2, the silhouette score in elbow method is given. In Figure 3 and 4. the customer picture and credit picture are given. We can see that the division result is good and reasonable. For example, cluster 1 customer is definitely high risk group, a large amount of them don't have own house. Credit purpose is mostly for car and radio/TV, therefore, this kind of customer belongs to high risk.

![Silhouette_Score](../../../../../figure/Silhouette_Score.jpg)
<center>Figure 2: Silhouette score for different clustering numbers. The inertia becomes stable from 4 clusters. </center>

![Four_Categlories_Customer_Picture](../../../../../figure/Four_Categlories_Customer_Picture.jpg)
<center>Figure 3: Customer picture for the four divided categlories.jpg. </center>

![Four_Categlories_Customer_Credit_Picture](../../../../../figure/Four_Categlories_Customer_Credit_Picture.jpg)
<center>Figure 4: Customer credit picture for the four divided categlories. </center>

To predict new customer risk, Random Forest model is chosen. The number of clustering is reset to be 2: high-risk and low-risk group, then is used for the training. Training and testing data is splitting with 7:3 ratio, and resampling is applied to avoid biased training.

The quality of training is given by accuracy, precision and recall. In Figure 5, the confusion matrix is given for the test data. 

![Confusion_Matrix](../../../../../figure/Confusion_Matrix.jpg)
<center>Figure 5: Confusion_Matrix.jpg. </center>

To measure the credit risk, the top 5 sensitive features are: Credit amount, Duration, Job, Age, Saving accounts.


