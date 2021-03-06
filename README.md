# Object Avoidance and Detection for Blind People
## Objective
The goal of the project is to develop a device that allows visually impaired people navigate around without much dependence on other people or cumbersome tool. It also helps the blind get more insight into the surroundings and locate specific objects with ease. 

We're using [Intel RealSense depth camera D435](https://www.intelrealsense.com/depth-camera-d435/) for object avoidance and detection tasks. The camera sends images and depth details to [Jetson Nano](https://www.nvidia.com/en-us/autonomous-machines/embedded-systems/jetson-nano/), a powerful microcomputer developed by Nvidia, for real-time processing. The camera and processor weigh approximately 50 grams in total, making it an extremly small and lightweight device that is comfortable to carry around. 

## Requirements
Hardware
- [Intel RealSense depth camera D435](https://www.intelrealsense.com/depth-camera-d435/)
- [NVIDIA Jetson Nano](https://www.nvidia.com/en-us/autonomous-machines/embedded-systems/jetson-nano/)

Software 
- [Intel Realsense SDK 2.0](https://github.com/IntelRealSense/librealsense) (compute real-time depth images)
- [OpenCV 4.1.1 with extra modules](https://github.com/opencv/opencv) (object detection and image captioning)

## Features
There're 3 features:
- [Obstacle Avoidance](#obstacle-avoidance)
- [Find objects](#find-objects )
- [Describe the surrounding environment](#describe-the-surrounding-environment)

### Obstacle Avoidance
As the user moves, the device detects the obstacles in the person view and then signal the user about them by generate the "beep" sounds. The closer the object, the louder and faster the sound is. The system also keeps track of the velocity of the moving objects in order to avoid sudden collision. 

### Find objects 
"Where is my wallet?", "Where is my yellow hat?", "Where are my jeans?"
</br>This project is the answer to these questions. The user can ask questions to .., and the device will analyze the voice and give instructions where to find the objects through the hearing device.  

### Describe the surrounding environment
With a view to providing the users more insight into their surroundings, we implement image captioning feature to describe the front view of the user. 








