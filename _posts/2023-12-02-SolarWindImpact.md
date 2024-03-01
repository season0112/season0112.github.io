---
layout: post
comments: true
title: Analysis of Solar Wind impact on Cosmic Rays
categories: [Cosmic Ray Analysis Project]
---

<!-- url is: /home/category/year/month/day/XXX.html -->

### Goal

Galactic cosmic rays are produced from supernova or interactions with interstellar medium. When they enter the galaxy, they would be affected by the solar wind, which is emitted from sun corona and has a periodicity of 22 years related to solar magnetic field. Due to the rareness of antiproton component in cosmic rays, its impact from solar wind has never been observed before.

### Analyasis

The analysed data are collected from AMS-02 detectors installed on the International Space Station from May. 2011 to May, 2021. Figure 1 shows the AMS-02 detectors in space. After data cleaning and reduction, higher level variables are constructed like Likelihood estimator based on the response of the detectors. 

![SolarWindImpact_AMS02](../../../../../figure/SolarWindImpact_AMS02.jpg)
<center>Figure 1: AMS-02 detectors installed on the International Space Station. </center>

Because the complex response of the detectors,  particle by particle identification is not possible, therefore, advanced statistical methods like Maximum Likelihood Fit is performed to extract signals numbers and the background numbers from the 200 billion collected particles. In Figure 2, an example Fit is shown as an example. The histograms are taken from Monte Carlo simulations, and black points are from collected data from detectors installed on the International Space Station. The antiproton (blue) signal distribution is different from electron (red) background distribution.

![SolarWindImpact_TemplateFit](../../../../../figure/SolarWindImpact_Templatefitplot.png)
<center>Figure2: Maximum Likelihood Fit on TRD Likelihood dimension to extract signal and background numbers. x axis is Constructed Estimator, Y is number of particles.</center>

### Result

The number ratio of the antiproton to proton components is shown in the Figure 3, the fluctuation is due to the solar magnetic activity and clearly visible here. This phenomena is firstly observed by human and of greatly value for solar physics.

![SolarWindImpact_FluxRatio](../../../../../figure/SolarWindImpact_FluxRatio.png)
<center>Figure 3: antiproton to proton ratio as a function of time. </center>