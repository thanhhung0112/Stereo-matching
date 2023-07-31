## Introduction
This repository aims to compute the disparity map between left and right image with differences in brightness via some common method `L1`, `L2`, `Cosine Similarity` and `Correlation Coefficient`
## Getting started
* My program is executed through Google Colab, so just uploading .ipynb file to Colab and running it
* There are total of 5 problems:
  + Using L1 and L2 with pixel-wise between 2 images to get the disparity map
  + Using L1 and L2 with RoI represented with kernel size value to get the disparity map
  + Apply to the left and the right image with different brightness to evaluate performance of L1 and L2
  + Using Cosine similarity with RoI represented with kernel size value to get the disparity map from the left and the right image with different brightness
  + Using Correlation coefficient instead of Cosine similarity and compare the achieved results
* In addition, with the problems using RoI, i apply an integral mechanism to optimize a computational cost. You can see what it is with the following image.
  
![Integral](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/b78bd17e-caff-48c7-a2dd-0cbf6e090568) ![Formula](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/7e6ecdff-4f64-4c95-b8ac-14dfd5c8d082)

## Results
|Method, Disparity Range, Kernel, Brightness|Result|
|-------|------|
|`L1`, `16`, `None`, `Same`||

  
