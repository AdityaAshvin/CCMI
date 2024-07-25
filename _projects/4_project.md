---
layout: page
title: Active speaker detection
description: Automatic visual detection of persons actively speaking on screen
img: assets/img/project4-img.png
importance: 3
category: past
---

## Project Description

“When” and “where” are the fundamental pillars of Computational Media Intelligence for developing a holistic understanding of a scene, which translates to locating the action of interest in both space and time. In this project, we develop a system to automatically detect the active speakers in space and time, specifically for media content.

## Methodology

This work is inspired by our preliminary work [1], where we presented a cross-modal system for the task of voice activity detection by observing just the visual frames. We performed a thorough analysis and showed that the learned embeddings can locate the human bodies and faces. The cross-modal architecture is shown below:

<img src="{{ site.baseurl }}/assets/img/project4-img1.png" alt="Methodology image" width="600">

## Demonstration of the System Output

The heatmaps represent the intermediate output of the system, signifying the salient regions in the visual frames pertaining to active speakers. The active speakers are shown in green bounding boxes and all other faces in blue.

## Video Demonstration

<video width="640" height="360" controls>
  <source src="{{ site.baseurl }}/assets/video/demo_as.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

## References

1. R. Sharma, K. Somandepalli, and S. Narayanan, “Toward Visual Voice Activity Detection for Unconstrained Videos,” 2019 IEEE International Conference on Image Processing (ICIP), 2019, pp. 2991-2995, doi: [10.1109/ICIP.2019.8803248](https://doi.org/10.1109/ICIP.2019.8803248).

2. Sharma, Rahul, Krishna Somandepalli, and Shrikanth Narayanan. “Crossmodal learning for audio-visual speech event localization.” *arXiv preprint arXiv:2003.04358* (2020).