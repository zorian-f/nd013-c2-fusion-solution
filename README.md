# SDCND : Sensor Fusion and Tracking

Write a short recap of the four tracking steps and what you implemented there (EKF, track management, data association, camera-lidar sensor fusion). Which results did you achieve? Which part of the project was most difficult for you to complete, and why?:


Do you see any benefits in camera-lidar fusion compared to lidar-only tracking (in theory and in your concrete results)?:

Which challenges will a sensor fusion system face in real-life scenarios? Did you see any of these challenges in the project?
Can you think of ways to improve your tracking results in the future?:
* In rela-Life a big challenge ist to compute in real-Time.

## Step 1

<p float="left" align="middle" width="99%" >
  <img src="img/Step1_plot.png" width="99%"/>
</p>

## Step 2

<p float="left" align="middle" width="99%" >
  <img src="img/Step2_plot.png" width="99%"/>
</p>

## Step 3

<p float="left" align="middle" width="99%" >
  <img src="img/Step3_plot.png" width="99%"/>
</p>

## Step 4

<p float="left" align="middle" width="99%" >
  <img src="img/Step4_plot.png" width="99%"/>
</p>

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
