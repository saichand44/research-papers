# Research Papers

This repository contains `research papers` related to robotics.

[1] [Local_INN: Implicit Map Representation and Localization with Invertible Neural Networks](https://ieeexplore.ieee.org/document/10161015)

`Authors`: Zirui Zang; Hongrui Zheng; Johannes Betz; Rahul Mangharam

`DOI`: 10.1109/ICRA48891.2023.10161015

`Summary`: <div align="justify"> Use an INN network to map the robot's poses and the LiDAR scans. After training, network gives out an estimate of the distribution of the robot's poses for a given LiDAR scan information. To make sure the inputs and the outputs are of same dimensions in the network, `positional encoding` is used for robot's poses (to ↑ dimensions) and `VAE` is used for LiDAR scans (to ↓ dimensions). This distribution of estimated poses can be used in filtering techniques for improving the state estimation. The network also needs information of the previous state along with the LiDAR data to output the robot's poses distribution. Likewise, during training, we need the previous state information to map the robot's pose and the LiDAR scans. </div>

---
