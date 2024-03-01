---
layout: post
comments: true
title: Cosmic Ray identification with Machine Learning
categories: [Cosmic Ray Analysis Project]
---

### Goal

The component of cosmic rays is complicated, including matter and anti-matter. The precise identification of anti-matter component is vital to understand our universe and investigate Dark Matter models.

The antiproton component is the second largest anti-matter component in the cosmic rays, but still contributes at 0.01\% level. Therefore, it is very rare and it's difficult to extract signal from the whole cosmic dataset.

### Using Machine Learning method to analyse

To identify Antiproton signals, the key issue is to separate them from backgrounds of Electrons and Charge Confused Proton(charge wrongly constructed protons). The behavior of signal and backgrounds are well understund by Monte Carlo Simulations data.

With the help of Monte Carlo Simulations data, a classifier has been obtained in supervised training. Different machine learning methods are used, and optimation of performance has been performed by parameter grid search. The input parameters are construted based on detector responds. In Figure 1, four example variable distributions (Rigidity Asysmmetry, Upper Lower Match, Chi2 Asysmmetry, Inner Rigidity Match) of signal and background are given to illustrate the separation information used for training.  

![CRMachineLearning_Input](../../../../../figure/CRMachineLearning_Input.png)
<center>Figure1: Four example variable distributions based on detector response of signal and backround.</center>

In the Fiture 2, the performance of different machine learning methods is given regarding to rejection power. In this case, the Neurl Network method achieves best performance. In Figure 3, the separation between signal and backrounds is achived with parameter optimised.

![CRMachineLearning_FractionFigure](../../../../../figure/CRMachineLearning_FractionFigure.png)
<center>Figure2: Rejection Power of different machine learning methods as function of efficiency.</center>

![CRMachineLearning_Separation](../../../../../figure/CRMachineLearning_Separation.png)
<center>Figure3: Separation between signal (Charge Correct) and background (Charge Confused).</center>
