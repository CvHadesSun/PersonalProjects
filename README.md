<!--
 * @Date: 2022-09-20 10:30:51
 * @LastEditors: cvhadessun
 * @LastEditTime: 2022-09-20 18:40:53
 * @FilePath: /PersonalProjects/README.md
-->
# PersonalProjects

## EPNet
![framework](assets/E2P/framework.png)
![ycb](assets/E2P/ycb-2.gif)

In this article, several previous work are referred to improve the efficiency of the algorithm to better serve complex scenarios, We use a two-stage pipeline to obtain the high-precision pose of the multi-object, in which the first stage is the key point detection, and the second stage solves PnP to obtain the 6DoF pose. We propose a simpler and more efficient classification-based key point detection algorithm for key points on the object surface. Experiments show that the proposed method outperforms the SOTA methods and robust on the LINEMOD, Occlusion-LINEMOD, and YCB-Video datasets. Especially, we outperform the SOTA methods on the challenging Occluded-LINEMOD dataset by a large margin. Our approach is more robust to occlusion and more efficient to multi-object pose estimation task. The code will be available at: https://github.com/CvHadesSun/E2P.


## Bazepose-Replementation

![framework](assets/blazepose/tracking_demo.png)

![landmark-lite](assets/blazepose/landmark_lite.png)

![demo](assets/blazepose/exercise_pose.gif)

[1] [blazepose](https://arxiv.org/pdf/2006.10204.pdf)

## PG-engine
The engine to generate human pose dataset based on blender.(blender2.92 or higher).  Committed to  more reality human render engine.

screen-shot
![blender](assets/pg-engine/blender.png)

![example](assets/pg-engine/00.gif)


### Framework

### 1.ENGINE

- [x] Scene : Init the overall scene of blender and input into Render to render source.
- [x] Material : Self-defined shading of blender(osl) to process: (**need to develop it for more reality pose**)
  -  Textures of 3D model
  -  Lights of scene
  -  Other material opertaion.
- [x] Render : Using blender engine to render animation.
- [x] Model : The object and animation engine.
  - [x] SMPL
  - [x] SMPL-X
  - [ ] Self-designed model

### 2.INPUT

- bg figures: the background  of scene  
- uv textures : 3D model's textures
- lights: the scene's lights
- camera: multi-view or single-view camera parameters
- pose ( +shape) data. : antimation input data.

### 3.OUTPUT

- [x] video: .mp4
- [x] images 
- [x] labels


## RepCount
1. To do cycle motion count with KNN classifier:
![knn](assets/repcount/test008_output.gif)

2. RPnet:To do cycle motion count with DL

![repnet](assets/repcount/image-20220117191327821.png)
![result](assets/repcount/output.gif)


## Multi-RGBD-PIFu


![system](assets/pifu/system_pifu.png)


