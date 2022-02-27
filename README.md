# ITK 3D Image Registration

This repository contains python script, dataset, and results of image registration performed using ITK python library. 

## Dataset

T1-Weighted MRI and T2-Weighted MRI volumes from a same subject acquired as a part of Female data set of Visible Human Project.

![](Fixed_image.gif)

![](Moving_image.gif)
Initially, there is small different in orientation between the two volumes. 

Red = T1-Weighted MRI
Blue = T2-Weighted MRI
![](Before_registration.gif)

## 3D Image Registration

Registration is performed in order to discover the best transformation that aligns the regions of interest in the supplied images. Translation registration is carried out to register two MRI volumes using the registration methods of ITK python package. In this assignment, T2-Weighted MRI volume is registered to T1-Weighted MRI volume.

Fixed Image = T1-Weighted MRI
Moving Image = T2-Weighted MRI
Initial transformation = Translation transform
Optimizer = Gradient descent 
Interpolator = Nearest neighbor 
Similarity metric = Mutual information

## Results 

Red = Fixed Image
Blue = Resampled Moving Image
![](After_registration.gif)

## Impact of Image Registration - Comparision

The fixed, moving and moving resampled  images are compared using 3D Slicer software tool. 
![](Comparsion.gif)

## Evalution 

Image registration is validated by visual insepection and results of automatic registration feature of ITK-SNAP software. 

![](Evaluation.gif)