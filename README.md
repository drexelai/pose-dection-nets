# Pose Detection:

Drexel AI 2023 Spring Project

## Introduction:

## Background
https://arxiv.org/pdf/1808.09568.pdf

## Methods

### Data
https://drexel0-my.sharepoint.com/:u:/g/personal/az548_drexel_edu/Ee-4nyzqx75JurbGzTv246EB_bcG4-A9827G9AwMuT5gyQ?e=Laa7Ls

https://cydar.ist.psu.edu/emotionchallenge/index.php

### Models: 
* MediaPipe
* 3D classifier (CNN or Sparse coding)

For each dataset:
* Use MediaPipe to track detailed facial and body features
* Pass the information from each frame to the 3D classifier
* Output is one hot vector and 3 scalar values
