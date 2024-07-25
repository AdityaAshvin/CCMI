---
layout: page
title: Subtitle Aligned Movie (SAM) Corpus
description: A large-scale dataset for speech activity detection in movies
img: assets/img/project9-img.jpg
importance: 4
category: past
---

# Project Description

SAM Corpus consists of speech segments from over 500 top-grossing Hollywood movies spanning 5 years (2014-19). Easily scalable techniques are employed to align movie audio to subtitles, which are then used to develop Speech Activity Detection (SAD) models.

## Gentle Alignment

Speech boundaries in movie audio are demarcated using an automatic alignment tool called Gentle. Gentle aligns a text transcript to the corresponding audio at the phoneme level, resulting in accurate word boundaries for successfully aligned words. We use subtitles extracted from OpenSubtitles as text input to Gentle. Around 70% of all words in the transcript are successfully aligned using this method, resulting in over 650K audio-words.

<img src="{{ site.baseurl }}/assets/img/project9-img1.svg" alt="Methodology image" width="600">

## Inter-Pausal Units (IPUs)

IPUs are short segments of contiguous speech separated by pauses. An IPU is characterized by two threshold values: pause duration (PT) and segment length (ST). After gentle alignment, consecutive aligned words are grouped together into IPUs which are at least ST seconds long. Two consecutive words belong to the same IPU if they are no more than PT seconds apart. Constructing IPUs in this fashion enables “segment” level processing, which is not only computationally efficient but also captures context useful for several downstream tasks.

<img src="{{ site.baseurl }}/assets/img/project9-img2.svg" alt="Methodology image" width="600">

## Dataset Stats

- **500+** Movies  
  Data from over 500 top-grossing Hollywood movies

- **225 Hours**  
  225 hours of gentle-aligned speech

- **275K+ IPUs**  
  Over 275K IPUs of duration 1.25s or longer

## Network Architecture

CNN architectures for Speech Activity Detection

<img src="{{ site.baseurl }}/assets/img/project9-img3.svg" alt="Methodology image" width="600">

On the right, we see the visualization of the activation maps from the CNN-GAP model architecture. For speech segments, the model attends to lower frequency regions corresponding to the first few harmonics. In contrast, for noise regions, the model attends to higher frequencies that correspond to non-speech sounds.

## Results

- **Benchmark Dataset:** AVA

## Summary

Automatic, easily scalable methods are used to extract reliable speech data from a large number of movies for training SAD models. Using novel CNN architectures, we show state-of-the-art performance on two benchmark movie datasets.

## Related Links

- [GitHub - Speech Activity Detection in Movies](https://github.com/usc-sail/mica-speech-activity-detection/wiki)

### Features

- [Download log-mel features from SAM-C](https://drive.google.com/file/d/1hz9zKtR4w8EiKCZ3klxqEZ4pHw3eXEnx/view)

### Publications

[1]. Hebbar, R., Somandepalli, K., & Narayanan, S. “Robust speech activity detection in movie audio: Data resources and experimental evaluation.” IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), 2019.