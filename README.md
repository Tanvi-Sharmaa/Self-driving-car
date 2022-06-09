# Self-driving-car

## Introduction:
A self-driving car, also known as an autonomous car or driverless car, is a vehicle that can travel between destinations without the need of any human effort. They can process streams of data from different sensors such as cameras, LiDAR, RADAR, GPS, or inertia sensors. This data is then modeled using deep learning algorithms, which then make decisions relevant to the environment the car is in. 

This repository consists of three sections: 
1. Road lane detection using Computer Vision. 
2. Object detection using YOLOv3 algorithm.
3. Traffic signs detection using Convolutional Neural Networks (CNN).

This work was done as exploratory project Under the supervision of Prof. Rakesh Kumar Mishra on the topic of "SELF DRIVING CAR" 
by
- Tanvi 
- Muskan
- Lavi Goyal


# TASK : LANE DETECTION
One of the many steps involved during the training of an autonomous driving car is lane
detection, which is the preliminary step.:

<p align = "center">
<img src ="https://github.com/Tanvi-Sharmaa/Self-driving-car/blob/main/lane%20detection%20steps.png" align = "center"/>
</p>
<br>

## Results for Lane Detection
https://user-images.githubusercontent.com/97230066/172736335-19eba72c-0df6-4cc2-bba8-0948f90ffebc.mp4


# TASK : OBJECT DETECTION
Object detection is also one of the critical components to support autonomous driving.
Autonomous vehicles rely on the perception of their surroundings to ensure safe and robust
driving performance. This perception system uses object detection algorithms to accurately
determine objects such as pedestrians, vehicles, traffic signs, and barriers in the vehicle's vicinity

For this we have used YOLOv3 along with open cv to detect objects.

## Results for Object Detection
https://user-images.githubusercontent.com/97230066/172734483-98bdba4b-5118-4199-9c88-74289763c4a4.mp4


## What is YOLO ?
• YOLO (You Only Look Once) is an algorithm that detects and recognizes various objects
in a picture (in real-time). Object detection in YOLO is done as a regression problem and
provides the class probabilities of the detected images.
  
• YOLO algorithm employs convolutional neural networks (CNN) to detect objects in
real-time. As the name suggests, the algorithm requires only a single forward propagation
through a neural network to detect objects.
  
• This means that prediction in the entire image is done in a single algorithm run. The CNN
is used to predict various class probabilities and bounding boxes simultaneously.
  
• The YOLO algorithm consists of various variants. Some of the common ones include tiny
YOLO and YOLOv3.

## Benefits of YOLO:
It has high Speed, High accuracy and Learning capabilities
  
## Architecture:
This architecture takes an image as input and resizes it to 448*448 by keeping the aspect ratio
the same and performing padding. 

This image is then passed in the CNN network. This model has 24 convolution layers and 4 max-pooling layers followed by 2 fully connected layers. To
reduce the number of layers (Channels), we use 1*1 convolution followed by 3*3 convolution.
This is done by generating (1, 1470) from the final fully connected layer and reshaping it to size (7, 7, 30).
This architecture uses Leaky ReLU as its activation function in the whole architecture except for the layer where it uses a linear activation function.
  
# Task: ROAD SIGN DETECTION AND RCEOGNITION
Traffic-sign recognition is a challenging subject and also a valuable subject in traffic engineering
research. Traffic signs contain necessary messages about vehicle safety and they show the latest
traffic conditions, define road rights, forbid and allow some behaviors and driving routes, etc.

## Solution:
We have used CNN based on a transfer of learning method for detection of traffic signs. Deep
CNN is trained with a big data set, and then effective regional convolutional neural network
(RCNN) detection is obtained through a spot of standard traffic training examples.

## What is CNN?
A convolutional neural network (CNN) is a type of artificial neural network used in image
recognition and processing that is specifically designed to process pixel data.
CNN is very similar to the brain as it also has neurons which in turn have weights and biases.
Each neuron receives an input on which it performs some operation, and the output is passed as
the input to the next neuron. It can have many layers, the first is the input layer, and the last is the
output layer. Anything else in between is called a hidden layer.

## Results for Road Sign Detection and Recognition
  <table>
  <tr>
    <td align = "center"><B>Input</B></td>
    <td align = "center"><B>Output</B></td>
  </tr>
  <tr>
    <td><img src = "https://github.com/Tanvi-Sharmaa/Self-driving-car/blob/main/road_sign_detection_i1.jpeg" height = "350", width = "450"/></td>
    <td><img src = "https://github.com/Tanvi-Sharmaa/Self-driving-car/blob/main/road_sign_detection_i2.jpeg" height = "350", width = "450"/></td>
 </tr>
  </table>
    
# Results and Conclusion:
Road lanes, obstacles around the car and traffic signs detection is a requisite part of autonomous
driving.
Lane detection which was done using computer vision identified the lanes properly.
Yolo v3 algorithm which was used for object detection has high speed, accuracy and learning
capabilities. However, the algorithm struggles to detect small objects and low-resolution objects.
Moreover, the yolov3 trained model may not be ideal when large datasets are hard to obtain.
    
Accuracy of 98.9% was achieved using the CNN trained model for traffic sign detection. One of
the limitations of the model is that it cannot be trained on a different dimension of images. So it
is mandatory to have same dimension in the dataset. Another limitation is that due to a large
number of classes it was not able to predict a few traffic signs correctly.
    
Autonomous vehicle technology is not yet mature enough. Still, it needs rigorous exposure to a
wide range of traffic, landscape, and natural conditions in which the autonomous vehicles can be
trained to perform as expected in actual traffic conditions.
