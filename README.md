# Deep-Learning-for-Self-Driving-Cars

**Problem Statement**

Building a prototype of a 1/10th autonomous car using state of the art Deep Learning techniques and Computer Vision. Deploying the trained model on Nvidia Jetson TX2 for real-time object detection.

**Hardware used**

NVIDIA Jetson TX2, Arduino, LIDAR sensors, IMU Sensor
Tools, Languages and Libraries used: Gym gazebo, Robotic Operating System, Python, C++, TensorFlow, OpenCV

This research is done for the Networked Robotic Systems Laboratory at Pennsylvania State University and is scheduled in the following parts:

1) A thorough Literature Review of conventional and state of art techniques used in Autonomous
Vehicles.
2) Built a lane detector using OpenCV.
3) Designed an AutoEncoder to detect and draw lanes. Final Mean Squared Error observed was 0.012.
4) Implemented the architecture of “Traffic Sign Recognition with Multi-Scale Convolutional Networks” by Pierre Sermanet and Yann LeCun to classify road traffic symbol of "German Traffic Sign Classifier".
Training accuracy obtained was 98.7% and testing 94.5%
5) Behavioural Cloning: Dataset is generated using Unity Simulator. By running the car on training track I gathered roughly around 5000 samples. Data processing step involves cropping, resizing, RGB to YUV conversion, flipping, adjusting brightness, shadowing, equalizing histogram, blurring, this increases training dataset samples (roughly 25000 samples). Trained the Nvidia CNN model for predicting steering angle.
6) Implemented real-time Yolo v2 model for object detection, but the model is heavy to be deployed on Nvidia Jetson TX2 as it uses VGG-16 as its base model.
7) Finally, implemented MobileNet Single Shot Multibox Detector and deployed on Nvidia Jetson TX2.
8) Successfully applied transfer learning on the Mobilenet Single Shot Multibox Detector model for detecting road symbols.
9) First one to deploy this architecture on Nvidia Jetson TX2. The training was stopped when the error reached 1, inference time of this model is 196 ms.

Worked with the Advanced Vehicle Team (AVT) at Pennsylvania State University as a Deep Learning Engineer.

If there's a problem in viewing the above videos, try this link: https://drive.google.com/open?id=1KV35BoQvipG5xwInpfhdR28O2lC4ZAOY
