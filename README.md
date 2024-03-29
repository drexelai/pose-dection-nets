# Pose Detection:

Drexel AI 2023 Spring Project

### This project is discontinued

## Introduction:

## Background
https://arxiv.org/pdf/1808.09568.pdf

## Methods

### Data
https://drexel0-my.sharepoint.com/:u:/g/personal/az548_drexel_edu/Ee-4nyzqx75JurbGzTv246EB_bcG4-A9827G9AwMuT5gyQ?e=Laa7Ls

https://cydar.ist.psu.edu/emotionchallenge/index.php

### Models: 
* YOLO, MoveNet, PoseNet (Getting pose coordinates)
* Transformer models (classification task)

### Tasks:
April 17th
* Literature review of current methods -> Outline important findings (Everyone)
  * Pose classification
  * Pose estimation
* Understanding the BoLD dataset (Alex)
* Look through examples of pose estimation and classification (Arjit, Bobby, Alisha)

April 24th
* Steven will run Alex's model for pose estimation
* Alisha will run MoveNet model for pose estimation
* Look into Omnipose and RSN (figure out if it's pretrained, look into features) -> Yashoda
* Multi-person pose estimation? -> Arijit
* Alex will look into MediaPipe and more detailed pose estimation

Potential models for classification 
* Temporal CNN
* Transformer

For next meeting:
* Compare outputs from each of the models
* If outputs are good, move onto classification

May 4th
* Alex - Finalize pipeline for encoding coordinates for each frame for each video, read TCN's https://arxiv.org/pdf/1703.10898.pdf
* Steven - Run Coordinate encoding pipeline
* Rithvik - Temporal Segment Networks
* Anyone - Prototypical Cross-Attention Networks for Multiple Object Tracking and Segmentation vis.xyz/pub/pcan/

* Everyone new to CNN's: 
  * https://www.tensorflow.org/tutorials/images/cnn
  * https://poloclub.github.io/cnn-explainer/

Important:
for every v that is 0, xyz are also 0

1d convolution on 2d grid
to shrink temporal dimension to 1x1xfeature maps -> spacial convolution ->feedforward network

also could use attention mechanism & transformer instead of spacial

seperate vs sequential convolutions for temporal and spatial
