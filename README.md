# SDCND : Sensor Fusion and Tracking

Write a short recap of the four tracking steps and what you implemented there (EKF, track management, data association, camera-lidar sensor fusion). Which results did you achieve? Which part of the project was most difficult for you to complete, and why?:
* In the EKF Step, i impelented a 3D EKF Filter analogues to the 2D one in the lessons. Because everything is mathematically well described as matrices, going from 2D to 3D is no big Problem. Only the transfer function `F` and the covariance `Q` need some attention.
* In implementing the track management, on challenge is to find the right heuristics for initializing, deleting und updating the tracks.
*  Most difficult was to understand how all the different Variables of the EKF play together. Especially to understand the non-linearity of the Camera measurement.
* In the end the model can successfully track 3 Targets without losing them once, it also deletes ghost-tracks or the ones which are out of sight. 

Do you see any benefits in camera-lidar fusion compared to lidar-only tracking (in theory and in your concrete results)?:
* The fusion definitive adds complexity if this added complexity is worth the benefist of having, e. g.  redundancy for me is not clear now. As i heard in the lessons, there are companies like Tesla which think Lidar is not needed at all or are even obstructive.

Which challenges will a sensor fusion system face in real-life scenarios? Did you see any of these challenges in the project?
Can you think of ways to improve your tracking results in the future?:
* In rela-Life a big challenge ist to compute in real-Time.
* Tracking can be improved with better associtation algorithm like global nearest neighbor or having some sense of time

## Step 1
EKF tracking a single real-world target with lidar measurement input over time:
<p float="left" align="middle" width="99%" >
  <img src="img/Step1_plot.png" width="99%"/>
</p>

## Step 2
Track management to initialize and delete tracks, set a track state and a track score:
<p float="left" align="middle" width="99%" >
  <img src="img/Step2_plot.png" width="99%"/>
</p>

## Step 3
Single nearest neighbor data association to associate measurements to tracks with multi target tracking:
<p float="left" align="middle" width="99%" >
  <img src="img/Step4_plot.png" width="99%"/>
</p>

## Step 4
Added nonlinear camera measurement model:
<p float="left" align="middle" width="99%" >
  <img src="img/Step3_plot.png" width="99%"/>
</p>
Resulting Video:

<p float="left" align="middle" width="99%" >
  <img src="img/my_tracking_results.gif" width="99%"/>
</p>

# Midterm Project
This Section belongs to the Midterm project
## Visualize range image channels (ID_S1_EX1)
The Following Tasks were done:
	
* Convert range image “range” channel to 8bit
* Convert range image “intensity” channel to 8bit
* Crop range image to +/- 90 deg. left and right of the forward-facing x-axis
* Stack cropped range and intensity image vertically and visualize the result using OpenCV

<p float="left" align="middle" width="99%" >
  <img src="img/img_range.png" width="99%"/>
</p>

## Visualize point-cloud (ID_S1_EX2)
As part of this exercise, cars in the Piontcloud are identified to analyse which features are stable. If we have a look at the Pictures below we can identify the following features to be stable:
* Windows
* Overall shape of the Vehicle (e. g. roof- and hoodline)
* Tires

<p float="left" align="middle" width="50%" >
  <img src="img/pcl_cars/pcl_car1.PNG" width="49%"/>
  <img src="img/pcl_cars/pcl_car2.PNG" width="49%"/>
  <img src="img/pcl_cars/pcl_car3.PNG" width="49%"/>
  <img src="img/pcl_cars/pcl_car4.PNG" width="49%"/> 
  <img src="img/pcl_cars/pcl_car5.PNG" width="49%"/>
  <img src="img/pcl_cars/pcl_car6.PNG" width="49%"/>
  <img src="img/pcl_cars/pcl_car7.PNG" width="49%"/>
  <img src="img/pcl_cars/pcl_car8.PNG" width="49%"/> 
  <img src="img/pcl_cars/pcl_car9.PNG" width="49%"/>
  <img src="img/pcl_cars/pcl_car10.PNG" width="49%"/> 
</p>
