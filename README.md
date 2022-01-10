# Jetbot Navigation

This repository contains a step-by-step procedure to implement autonomous navigation for Nvidia Jetbot. The method uses a tiny DNN model of 0.5MB size to segment the road area from the calibrated image. 
Follow the steps below to implement the solution:
1. Camera Calibration: use the CameraCalibration.ipynb to obtain the calibration matrices for your camera.
2. Dataset: obtain calibrated images and develop segmentation ground truth. Based on the experiment, it has been found that 50 images are more than enough for a small road track environment.
3. Train DL model: use the developed dataset from the previous step to train a model for binary segmentation. Segmentation.ipynb available for your to obtain the necessary model. 
4. Navigate with the Jetbot: upload the model developed from the previous step on the Jetbot. Run the JetbotNavigation.ipynb from the repository and have fun. The robot will start to navigate based on the available space of the road. The robot will also do the necessary maneuver to follow the route.     
