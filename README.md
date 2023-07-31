## Introduction
This repository aims to compute the disparity map between the left and the right image with differences in brightness via some common method `L1`, `L2`, `Cosine Similarity` and `Correlation Coefficient`
## Getting started
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1chhuzy5PeVHVz9g8a26W0jlluJVOv-BV)
* There are total of 5 problems:
  + Using L1 and L2 with pixel-wise between 2 images to get the disparity map
  + Using L1 and L2 with RoI represented with kernel size value to get the disparity map
  + Apply to the left and the right image with different brightness to evaluate performance of L1 and L2
  + Using Cosine similarity with RoI represented with kernel size value to get the disparity map from the left and the right image with different brightness
  + Using Correlation coefficient instead of Cosine similarity and compare the achieved results
* In addition, with the problems using RoI, i apply an integral mechanism to optimize a computational cost. You can see what it is with the following image.
  
![Integral](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/b78bd17e-caff-48c7-a2dd-0cbf6e090568) ![Formula](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/7e6ecdff-4f64-4c95-b8ac-14dfd5c8d082)

## Results
|Method|disparityRange|Kernel|Brightness|Result|
|------|--------------|------|----------|------|
|`L1`|`16`|`None`|`Same`|![L1_range16](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/25350870-c5ed-480d-b5d3-c2377b8c7b33)|
|`L1`|`64`|`None`|`Same`|![L1_range64](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/4e5d3187-9307-4e07-9022-1a0a962f8d64)|
|`L2`|`16`|`None`|`Same`|![L2_range16](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/5d04dd9f-1628-48c7-9433-519e8726443b)|
|`L2`|`64`|`None`|`Same`|![L2_range64](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/b95c3424-97e7-4551-9e17-ff358c4a0ade)|
|`L1`|`16`|`5`|`Same`|![L1_range16_kernel5](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/02d3ebfd-e2c5-45a9-8b34-6fc0ad6179e1)|
|`L1`|`64`|`5`|`Same`|![L1_range64_kernel5](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/c5600751-94cb-4604-a236-21030790a814)|



  
