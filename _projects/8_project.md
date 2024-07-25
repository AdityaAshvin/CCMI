---
layout: page
title: Representation of Professions in Entertainment Media
description: Insights into Frequency and Sentiment Trends
img: assets/img/project8-img.png
importance: 2
category: past
giscus_comments: false
---

# Project Description

Media acts as a mirror to society. Societal trends and culture dictate media narratives, which in turn inform and mold our perception of the real world. We study media representation of professions and analyze its frequency and sentiment trends. Our findings reveal that professions frequently mentioned in media tend to employ more people.

## Short Demo

<video width="640" height="360" controls>
  <source src="{{ site.baseurl }}/assets/video/project8.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

### Profession Taxonomy

The profession taxonomy is organized into 3 tiers: SOC Groups, WordNet synsets, and professions. 

- **SOC Groups:** The outermost circles represent SOC Groups.
- **Synsets:** Click on a SOC circle to zoom into its synsets.
- **Professions:** Click on a synset circle to zoom into its professions.
- **Zoom Out:** Click outside the circle to zoom out.

### Subtitle Corpus

- **3.3M** Mentions  
  Professional Mentions

- **133K** IMDb Titles  
  Movies and TV Shows

- **68** Years  
  Time Range

## Method

<img src="{{ site.baseurl }}/assets/img/project8-img1.jpg" alt="Methodology image" width="600">

1. **Expansion of SOC Taxonomy:** We expand the SOC taxonomy by finding noun WordNet synsets of the SOC professions and include their synonyms and hyponyms. We map these professions and synsets to major SOC groups.

2. **Subtitle Corpus Search:** We search for mentions of job titles in the OpenSubtitles corpus. Mentions not belonging to our expanded taxonomy or names of persons cast in movies or TV shows are ignored. The resulting subtitle corpus of professional mentions is automatically annotated with targeted sentiment labels (positive, negative, or neutral) using a BERT-based sentiment analysis model trained on human-annotated subtitle sentences.

3. **Analysis:** We compute the frequency and sentiment trends of the top 500 occurring professions over time. We also study the effect of media attributes (genre, title type, and country of production) on these trends. Additionally, we analyze the correlation between mention frequency and employment of major SOC groups, observing that professions with higher employment are mentioned more frequently in media content.


## Download

- [GitHub - Profession Taxonomy and Subtitles Corpus](https://github.com/sabyasachee/mica-profession/tree/main/datasets)

For more information, find our [PLOS ONE paper here](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0267812).