# REAL_TIME_Distance-Estimation_Using_YOLOV5
YOLOER stands for You Only Look Once and Estimate Range while V1 implies the version of object detector (V1 = YOLOv5). The project is about REAL-TIME Object Detection and Distance/Depth Estimation using the YOLOv5 object detector. To test the Real-Time functionality immediately, we provide the option of running the model on the webcam. Moreover, the options of testing on recorded videos and images are also provided.  

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HassanBinHaroon/YOLOER_V1/blob/master/YOLOER_V1.ipynb)

# Demo 
Coming Soon  

## Table of Contents

 ### 1. Inference on Local Machine Webcam
 ### 2. Inference on Google Colab (quick start)
 ### 3. Training of Object Detector 
 ### 4. Training of Distance Estimator

## Inference on Local Machine Webcam

In order to test any Real-Time system, the most convenient method is to run on the webcam. So, we provide the options of quick inference on a local machine and visualization through the webcam. Some installations are required before running the inference and the following subsection contains the entire method. So follow step by step. 

Moreover, we prefer working in Conda environments and it is recommended to install it first. In case of not have Conda installed, just skip the Conda-specific commands and follow along.  

### Installation Procedure

#### Step 1

      conda create --name YOLOER_V1 python=3.7 -y && conda activate YOLOER_V1 
      
#### Step 2      
      
      git clone https://github.com/HassanBinHaroon/YOLOER_V1.git
      
#### Step 3

      cd YOLOER_V1/object-detector_PLUS_distance-estimator
      
#### Step 4

      pip install -r requirements.txt
      
#### Step 5

      python setup.py
      
#### Step 6

### Inference Execution Command

      python detect.py --save-txt --weights yolov5s.pt --conf 0.4 --source ../videos/car.jpg --model_dist model@1535470106.json --weights_dist model@1535470106.h5
      
## Inference on Google Colab (quick start)

Click on the following link.

https://colab.research.google.com/github/HassanBinHaroon/YOLOER_V1/blob/master/YOLOER_V1.ipynb

### Must Do After Clicking

#### >>>>> Change runtime type

![](https://github.com/HassanBinHaroon/YOLOER_V1/blob/master/images/im1.png)

#### >>>>> Select GPU

![](https://github.com/HassanBinHaroon/YOLOER_V1/blob/master/images/im2.png)

#### >>>>> Run All

![](https://github.com/HassanBinHaroon/YOLOER_V1/blob/master/images/im3.png)

### Results Visualization

![](https://github.com/HassanBinHaroon/YOLOER_V1/blob/master/images/results_vis.png)

Note! The project is still in progress. 
