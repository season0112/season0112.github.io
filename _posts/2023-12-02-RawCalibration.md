---
layout: post
comments: true
title: Raw Cosmic Ray data calibration
categories: [Science Data Calibration Project]
---

<!-- url is: /home/category/year/month/day/XXX.html -->

### Goal

The AMS-02 detectors are installed on the International Space Station. Due to the space environment change or issues like power cut on the Space Station, the detector performance has to be calibrated before it is used for data analysis. Figure 1 shows a cosmic ray travel through the detectors. As we observed here, there are many junks interaction in the reconstruction. This leads to a bias for a certain detector response.

![RawCalib_Event](../../../../../figure/RawCalib_Event.png)
<center>Figure 1: Visualisation of a beam of comic ray  going through the detectors (left) and physics variables measurement of this beam of comic ray. </center>

### Calibration Process

An example of the measurement before calibration is given in Figure 2, the position (left) and time (right) measurement on the day of 26.11.2013 is shown. Clearly a jump on the measurement is noticed on this day. The reason is a sub-detector power configuration change.

![RawCalib_Jump](../../../../../figure/RawCalib_Jump.png)
<center>Figure 2: Position (left) and time (right) measurement on 26.11.2013 before calibration. </center>

My responsibility is to calibrate one of the sub-detectors called ACC. The method is using other sub-detectors like Transition Radiation Detector, Time Of Flight, and Silicon Tracker to construct the particle trajectories, and use the golden construct as a reference to calibrate the time, position and charge measurement from the ACC.

In Figure 3, the position measurement after calibration is shown as a example. As shown in this figure, the jumps in the raw measurement is resolved and this calibrated measurement can be used in the analysis.

![RawCalib_After](../../../../../figure/RawCalib_After.png)
<center>Figure 3: Position measurement on 26.11.2013 after calibration. </center>