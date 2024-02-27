---
layout: post
comments: true
title: Analysis of Product Comments in Online Shopping Website
categories: [NLP Project]
---

<!-- url is: /home/category/year/month/day/XXX.html -->

JD.com is an online shopping website which ranks 7th worldwidely in 2021 by revenue. Cell Phone is one of the best selling product on this website. To understand the product quality, the user's comments on the purchased phone are collected for a sentiments analysis.

Source of data:  Comments from Phone Category JD.com Website. In total, 3000 comments are collected for this analysis. The data includes User Name, comment time, comment content etc.

To understand the user's feedback on the purchased phone, the sentiments of these comments have to be evaluated. The sentiments behind the comments are calculated using Bayesian algorithm. The implementation is provided by SnowNLP Library. 

In Figure 1, the sentiments score for the 3000 user comments are given in a histogram. Figure 2 shows the positive and negative comments percentages in these 3000 comments.

![Histogram_of_Emotion_Score](../../../../../figure/Histogram_of_Emotion_Score.png)
<center>Figure 1: Sentiments score for user comments. Here peak at 1 means positive comments; -1 means negative comments.  </center>

![PiePlot_PosNeg](../../../../../figure/PiePlot_PosNeg.png)
<center>Figure 2: Pie Plot for positive and negative comments percentages. </center>

To have a visualisation of the sentiments of these comments, "Jieba" Library is used to cut comments into words in a reasonable way. Then word cloud is used to visualise the key words in comments.

In Figure 3, WordCould for top words is created for the total comments. In Figure 4, WordCould for top words is created for the negative comments. We can see that among the words appeared in this WordCould, most of them are negative words. This gives us confidence that our sentiments evaluation is correct.

![WordCould](../../../../../figure/WordCould.png)
<center>Figure 3: WordCould for total comments. </center>

![PiePlot_PosNeg](../../../../../figure/NegativeWordCloud.png)
<center>Figure 4: WordCould for negative comments. </center>