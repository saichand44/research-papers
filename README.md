# Research Papers

This repository contains `research papers` related to robotics.

[1] [Local_INN: Implicit Map Representation and Localization with Invertible Neural Networks](https://ieeexplore.ieee.org/document/10161015)

`Authors`: Zirui Zang; Hongrui Zheng; Johannes Betz; Rahul Mangharam

`DOI`: 10.1109/ICRA48891.2023.10161015

`Summary`: <div align="justify"> Use an INN network to map the robot's poses and the LiDAR scans. After training, network gives out an estimate of the distribution of the robot's poses for a given LiDAR scan information. To make sure the inputs and the outputs are of same dimensions in the network, `positional encoding` is used for robot's poses (to ↑ dimensions) and `VAE` is used for LiDAR scans (to ↓ dimensions). This distribution of estimated poses can be used in filtering techniques for improving the state estimation. The network also needs information of the previous state along with the LiDAR data to output the robot's poses distribution. Likewise, during training, we need the previous state information to map the robot's pose and the LiDAR scans. </div>

---

[2] [iMAP: Implicit Mapping and Positioning in Real-Time](https://ieeexplore.ieee.org/document/9710431)

`Authors`: Edgar Sucar, Shikun Liu, Joseph Ortiz, Andrew Davison

`DOI`: 10.1109/ICCV48922.2021.00617

`Summary`: <div align="justify"> iMAP presents a `dense SLAM` method that works in real-time through continual learning of an `MLP` trained on the images taken by an RGB-D camera. Here, only the `MLP` is used in the contruction of the map / scene in realtime. This paper presents a mechanism that runs both `tracking` and `mapping` simultaneouly using the `MLP`, but at different rates. In the pipeline, when a new RGB-D image is given, an optimization is run along with `MLP` to estimate the best possible camera pose. This is the `tracking` phase. The same picture is used (if it satisfies keyframe criteria) to train the `MLP` network for improved accuracy in the `mapping` phase. To achieve real-time implementation, instead of using all the pixels for training the MLP / NeRF, only a select group of pixels are used via `Active Sampling` technique. A similar stratergy is used in choosing the keyframes for training the `MLP`.

![iMAP](https://github.com/saichand44/research-papers/assets/14955987/d518945f-35e2-402b-8652-227bb5d10224)

---
