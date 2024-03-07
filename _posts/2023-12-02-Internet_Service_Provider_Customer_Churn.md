---
layout: post
comments: true
title: Internet Service Provider Customer Churn 
categories: [Customer and Revenue Project]
---

<!-- url is: /home/category/year/month/day/XXX.html -->

This is a churn analysis of customer from internet service provider. The goal is to predict churn probability based on the customer attributes, and give suggestions for various customer portfolio groups.

Data Source: The data is from a telco operator and contains about customer subscription information including average billing amount, contract period, download and upload data etc.

In Figure 1, some customer attributes are shown for illustration. The correlations between them are given in figure 2.

![CustomerAttributes](../../../../../figure/Plot_number_data_.pdf)
<center>Figure 1: Customer attributes distribution. </center>

![Correlation](../../../../../figure/Plot_Correlation.pdf)
<center>Figure 2: Correlation Matrix between customer attributes variables. </center>

Split the customer data to training and test dataset, and train a KNN model to predict churn probability for each customer in the training dataset. In figure 3, the confusion matrix is given for the test sample.

![Confusion_Matrix](../../../../../figure/Confusion_Matrix_churn.pdf)
<center>Figure 3: Confusion Matrix on the test sample. </center>

To have further investigation on the customer data, a clustering is applied. The customer data is presented with a pivot table, and K-Means Clustering method is used to divide the customer into 6 distinct groups. The heatmap of the 6 groups is given in figure 4. 

![heatmap](../../../../../figure/heatmap.pdf)
<center>Figure 4: Heat Map on the clustered costomers. In the X axis, "C" is contract remaining period, "M" is amount of internet spending, "A" is the measure of activity, "S" is the measure of satisfaction, "L" is the client total subscription period.</center>







<!-- suggestion: promotions distribution? -->




