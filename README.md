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

<p align="center">
  <img src="https://github.com/thanhhung0112/Stereo-matching/assets/79474374/b78bd17e-caff-48c7-a2dd-0cbf6e090568">
</p>

<p align="center">
  <img src="https://github.com/thanhhung0112/Stereo-matching/assets/79474374/7e6ecdff-4f64-4c95-b8ac-14dfd5c8d082">
</p>

## Results
|Method|disparityRange|Kernel|Brightness|Result|
|------|--------------|------|----------|------|
|`L1`|`16`|`None`|`Same`|![L1_range16](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/25350870-c5ed-480d-b5d3-c2377b8c7b33)|
|`L1`|`64`|`None`|`Same`|![L1_range64](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/4e5d3187-9307-4e07-9022-1a0a962f8d64)|
|`L2`|`16`|`None`|`Same`|![L2_range16](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/5d04dd9f-1628-48c7-9433-519e8726443b)|
|`L2`|`64`|`None`|`Same`|![L2_range64](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/b95c3424-97e7-4551-9e17-ff358c4a0ade)|
|`L1`|`16`|`5`|`Same`|![L1_range16_kernel5](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/02d3ebfd-e2c5-45a9-8b34-6fc0ad6179e1)|
|`L1`|`64`|`5`|`Same`|![L1_range64_kernel5](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/c5600751-94cb-4604-a236-21030790a814)|
|`L2`|`16`|`5`|`Same`|![L2_range16_kernel5](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/1062b1df-08b8-4cf3-9803-d573b7739025)|
|`L2`|`64`|`5`|`Same`|![L2_range64_kernel5](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/f7c7c0dc-1c27-462a-b394-0794c9ee3764)|
|`L1`|`64`|`3`|`Light`|![L1_range64_kernel3_light](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/ba32ada4-7a13-4977-a5a8-7041a4d2f872)|
|`L2`|`64`|`3`|`Light`|![L2_range64_kernel3_light](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/9a922b05-e543-4c35-9d0b-1688f69bcaa1)|
|`Cosine`|`64`|`3`|`Light`|![Cosine_range64_kernel3_light](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/eda51014-0728-4094-b6c6-b97a207abf45)|
|`Cosine`|`64`|`5`|`Light`|![Cosine_range64_kernel5_light](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/152e763b-cf5f-405c-a549-016a9020f888)|
|`Cosine`|`64`|`3`|`Dark`|![Cosine_range64_kernel3_dark](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/0a023163-b29b-46e7-918b-a3eeae4d2a27)|
|`Coef`|`64`|`3`|`Light`|![Coef_range64_kernel3_light](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/565c3637-2b15-41cb-a9cb-9e74300755d7)|
|`Coef`|`64`|`5`|`Light`|![Coef_range64_kernel5_light](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/b2e6d5b8-2e99-49fe-8b2b-ceb23360ccca)|
|`Coef`|`64`|`3`|`Dark`|![Coef_range64_kernel3_dark](https://github.com/thanhhung0112/Stereo-matching/assets/79474374/fb9856b9-c009-4628-8dd2-07ea32003fbd)|

