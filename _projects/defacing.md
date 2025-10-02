---
layout: page
title: "Defacing Biases in Quality Assessments"
description: "Investigated impact of facial feature removal on manual and automated quality control of structural MRI."
img: assets/img/publication_preview/OriginalVSdefaced+background.png
importance: 2
category: work
tags:
  - statistics
  - quality-control
  - software-engineering
  - communication
---
# Technical Context
Defacing, the process of removing facial features from structural MRI images to protect participant privacy, was suspected to alter quality assessments of images. Through the investigation of a comprehensive imaging dataset combined with statistical analyses, we demonstrated that defacing significantly influences both human experts' perception of image quality and automated quality control tools, revealing a critical gap in neuroimaging data processing pipelines.

## What I did
- Designed and executed a controlled experiment comparing quality assessments on defaced vs. non-defaced T1-weighted images
- Recruited and trained four human raters to conduct consistent quality evaluations using standardized protocols
- Developed automated analysis pipeline using statistical modeling (linear mixed-effects models) to quantify defacing biases
- Implemented comprehensive data collection and annotation framework (Q'kay web application) for large-scale manual assessments
- Analyzed inter-rater and intra-rater reliability to establish robustness of quality assessment procedures

## Methods / Stack
- **Statistical Analysis**: Linear mixed-effects models, repeated-measures ANOVA, Bland-Altman plots for reliability assessment
- **Labeling Platform**: Q'kay web application for managing large-scale annotation tasks with quality control features
- **Defacing Tool**: PyDeface for facial feature removal with validation of successful processing
- **Quality Assessment**: MRIQC-generated visual reports and IQMs for both manual and automated evaluation
- **R Statistical Software**: Implementation of statistical analyses with lme4, rstatix, and effectsize packages

## Outcomes (tech-focused)
- Demonstrated significant defacing bias in human quality assessments using mixed-effects statistical models
- Quantified effect sizes showing substantial impact on image quality perception (partial eta-squared effect sizes)
- Developed standardized protocols for conducting reproducible quality assessment studies
- Created open-source tooling for managing large-scale annotation tasks with built-in quality control
- Established recommendations for neuroimaging data sharing to prevent quality assessment deterioration
- Contributed to understanding of how privacy protection measures can compromise data utility in research
- Improved reliability estimates for neuroimaging QA/QC procedures through robust statistical evaluation
