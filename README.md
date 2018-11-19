# PG-CNN
Code for our ICPR 2018 paper: "Patch-Gated CNN for Occlusion-aware Facial Expression Recognition"

The following figure shows how we select the ciritcal points to crop patches from a facial image:
![alt text](https://github.com/mysee1989/PG-CNN/blob/master/img/point.png)   
(a) denotes totally 30 landmarks within original 68 facial landmarks. These points are involved in point selection   
(b) shows 16 points that we pick to cover the facial regions on or around eyes, eyebrows, nose, mouth   
(c) illustrates four points that are recomputed to better cover eyes and eyebrows   
(d) displays four points that are re-computed to cover facial cheeks   
(e) shows the selected 24 facial landmarks, around which the patches in (f) are cropped   


**Training yourself**   
We designed caffe layer named by ***multi_roi_pooling_layer***. Currently the layer is provided with a GPU version.   
Building the ***multi_roi_pooling_layer*** with the related proto definition in proto folder, you can adopt the network definition file in prototxt folder for training immediately.

**Precautions**    
The training and testing image list should be arranged as 
