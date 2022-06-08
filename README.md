# Self-driving-car
# Road_Segmemtation

# Introduction:
A self-driving car, also known as an autonomous car or driverless car, is a vehicle that can travel between destinations without the need of any human effort. They can process streams of data from different sensors such as cameras, LiDAR, RADAR, GPS, or inertia sensors. This data is then modeled using deep learning algorithms, which then make decisions relevant to the environment the car is in. 

This repository consists of three sections: 
1. Road lane detection using Computer Vision. 
2. Object detection using YOLOv3 algorithm.
3. Traffic signs detection using Convolutional Neural Networks (CNN).
# Model Architecture:
<p align = "center">
<img src ="./architecture.jpg" align = "center"/>
</p>
<br>
In the above shown model, the pretrained VGG-16 networks are used as encoder. The VGG_16 was trained on pretrained on ImageNet for classification. The 
pretrained weights can be found on the link - <a href = "https://s3-us-west-1.amazonaws.com/udacity-selfdrivingcar/vgg.zip">Udacity Self Driving Car</a>

# Files and Folders:

<ol>
  <li><B>Dataset folder : </B>This folder contains the dataset.</li>
  <li><B>Masked Dataset folder : </B>This folder has the dataset in the masked form. The masking was done manually.</li>
  <li><B>Final Showdown folder : </B>This folder has final outputs or predictions by the model.</li>
  <li><B>FCN folder : </B>This folder has all the codes for the model.</li>
  <li><B>FCN_combo folder : <B>This folder contains the codes for both image and video predictions.</li>
  <li><B>Report_and_Results.pdf file : <B>This folder contains the report of the project.</li>
  <li><B>resize_red_masking.py : <B>This file is reponsible for resizing the image and making semanted mask of it.</li>
</ol>

# Installation :

Go to this link to see, how to train and predict from the model --->  <a href = "https://github.com/AYUSH-ISHAN/Road_Segmentation/tree/main/FCN#training--">For images</a> and <a href = "https://github.com/AYUSH-ISHAN/Road_Segmentation/tree/main/FCN_combo#training--">for Videos and Image</a>both predictions.

# Results on sample images:

<table>
  <tr>
    <td align = "center"><B>IMAGE</B></td>
    <td align = "center"><B>MASK</B></td>
    <td align = "center"><B>OUTPUT</B></td>
  </tr>
  <tr>
    <td><img src = "./dataset/umm_road_1.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/umm_road_1.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/umm_road_1.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/umm_road_5.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/umm_road_5.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/umm_road_5.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/umm_road_valley.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/umm_road_valley.png"/ height = "150", width = "250"></td>
    <td><img src = "./Final_Showdown/umm_road_valley.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/umm_road_10.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/umm_road_10.png"/ height = "150", width = "250"></td>
    <td><img src = "./Final_Showdown/umm_road_10.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/umm_road_20.png"/ height = "150", width = "250"></td>
    <td><img src = "./masked_dataset/umm_road_20.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/umm_road_20.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/umm_road_40.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/umm_road_40.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/umm_road_40.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/umm_road_30.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/umm_road_30.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/umm_road_30.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/umm_road_1.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/umm_road_1.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/umm_road_1.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/forest_dataset/umm_road_4.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/forest_masked/umm_road_4.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/forest_final/umm_road_4.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/forest_dataset/umm_road_6.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/forest_masked/umm_road_6.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/forest_final/umm_road_6.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/forest_dataset/umm_road_66.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/forest_masked/umm_road_66.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/forest_final/umm_road_66.png" height = "150", width = "250"/></td>
 </tr>
  <tr>
    <td><img src = "./dataset/forest_dataset/umm_road_88.png" height = "150", width = "250"/></td>
    <td><img src = "./masked_dataset/forest_masked/umm_road_88.png" height = "150", width = "250"/></td>
    <td><img src = "./Final_Showdown/forest_final/umm_road_88.png" height = "150", width = "250"/></td>
 </tr>
  
 </table>

# Results on sample videos:

<img src = "./video_prediction.gif">
    
# References:
<a href = "https://github.com/JunshengFu/semantic_segmentation">Source 1</a><br>
<a href = "https://github.com/lb5160482/Road-Semantic-Segmentation/">Source 2</a>
