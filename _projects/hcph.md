---
layout: page
title: "Human Connectome Phantom Dataset"
description: "Designed and ran 72-session multimodal MRI acquisition and containerized preprocessing on HPC with reproducible versioning."
img: assets/img/publication_preview/HCPhDataset-small.png
importance: 1
category: work
tags:
  - data-engineering
  - acquisition-organization
  - quality-control
  - software-engineering
---
# Technical Context
The Human Connectome Phantom (HCPh) dataset addresses key challenges in connectivity reliability by featuring repeated scans of a single individual across three scanners using multi-echo functional MRI and multi-shell diffusion MRI. This design provides the unique opportunity to characterize the inter-scanner reliability of both functional and structural connectivity within a unified framework. The sessions on one scanner also incorporated extensive physiological monitoring and acquired the resting-state fMRI using a naturalistic paradigm to enable a detailed examination of intra-scanner variability.

## What I did
- Designed comprehensive multimodal MRI acquisition protocol involving structural, diffusion, and functional sequences with simultaneous physiological recording
- Coordinated 72-session data collection across multiple scanners while maintaining consistent experimental conditions
- Developed containerized preprocessing pipelines on HPC systems for scalable analysis of large neuroimaging datasets
- Implemented quality control protocols ensuring data integrity throughout the acquisition and analysis workflow
- Established reproducible versioning and documentation through Standard Operating Procedures

## Methods / Stack
- **MRI Sequences**: Multi-echo functional MRI (multi-echo EPI), multi-shell diffusion MRI (high-angular resolution diffusion imaging)
- **Physiological Monitoring**: ECG, respiration belt, exhaled CO2 concentration, eye tracking synchronized with image acquisition
- **Software Tools**: fMRIPrep, dMRIPrep, MRIQC for preprocessing and quality control
- **Containerization**: Docker for reproducible analysis environments
- **High-Performance Computing**: Optimization of pipelines for efficient processing on HPC systems

## Outcomes (tech-focused)
- Successfully acquired high-quality multimodal neuroimaging data across repeated sessions
- Established reproducible preprocessing workflows enabling consistent analysis across scanners and time points
- Developed comprehensive quality control protocols validated through systematic assessment procedures
- Demonstrated feasibility of longitudinal neuroimaging studies with integrated physiological monitoring
- Contributed to the characterization of scanner and temporal variability in brain connectivity measurements attraverso:
  - Inter-scanner reliability assessment across three different MRI systems
  - Intra-scanner reliability characterization over multiple acquisition sessions
  - Analysis of physiological influences on measured connectivity patterns
