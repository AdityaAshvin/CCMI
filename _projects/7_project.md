---
layout: page
title: Actions, Agents and Patients
description: A computational linguistic lens into gendered actions in film
img: assets/img/project7-img.jpg
importance: 6
category: past
related_publications: true
---

# Project Description

We develop models, data, and statistical analysis necessary to uncover the pervasiveness of stereotypical portrayals in characters’ actions at scale.

## Why Is It Important?

To understand the influential relation between exposure to media content and accepted social norms and expectations through large-scale quantitative measurements of characters’ attributes (e.g., age, gender, or race).

<video width="640" height="360" controls>
  <source src="{{ site.baseurl }}/assets/video/project7.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

## Dataset Stats

- **1.2M+** Sentences  
  Action descriptions

- **50k+** Actions  
  Distinct actions

- **25K+** Characters  
  Identified characters

## Automatic Identification of Characters and Actions

Our proposed SRL system operates as follows:

1. **Input:** An action description in natural language.
2. **Processing:** The BERT transformer creates a highly-contextualized representation for each word, encoding semantics and context.
3. **Modeling:** A recurrent neural network and a softmax layer for sequence labeling process the vector representations.
4. **Post-Processing:** Heuristics aggregate multi-word expressions to handle groups of agents or patients.

## Statistical Analysis

We use a Poisson-regression generalized linear mixed model (GLMM) to identify significant differences in action portrayals due to the role and gender of participants. GLMMs extend generalized linear models to include both fixed and random effects.

### Results

- **Agency:** Findings related to how agency is portrayed across different genders.
- **Male Gaze:** Analysis of gendered perspectives in media.
- **Disability:** Insights into the portrayal of disability.
- **Emotion:** Examination of emotional representations in characters.

**Example Finding:** Whenever a character requires someone to push their wheelchair, male agents are unlikely to ‘wheel’ either female or male patients.

## Summary

This work presents a novel large-scale analysis of actions taken by characters and how these actions are related to gender biases in media.

## Related Links

- [GitHub - Code Repo for Large-Scale Analysis of Characters’ Actions](https://github.com/usc-sail/mica-actions-agents-and-patients)