# Awesome Polyphonic Sound Event Detection

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![GitHub stars](https://img.shields.io/github/stars/LJF-SAL/awesome-polyphonic-sound-event-detection?style=social)

Curated reading list for **Polyphonic Sound Event Detection (Polyphonic SED)** methods, focused on the **DESED** dataset (DCASE Task 4). Organized by pipeline stages: Frontend → Model Architectures → Data Utilization → Post-processing.

**Last updated**: March 2026

Inspired by [soham97/awesome-sound_event_detection](https://github.com/soham97/awesome-sound_event_detection) (narrowed and restructured for DESED-specific methods).

## Table of Contents
- [Awesome Polyphonic Sound Event Detection](#awesome-polyphonic-sound-event-detection)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Survey Papers](#survey-papers)
  - [Datasets \& Benchmarks](#datasets--benchmarks)
  - [Frontend / Acoustic Features](#frontend--acoustic-features)
  - [Model Architectures](#model-architectures)
    - [CNN-based](#cnn-based)
    - [Pre-trained Models Fine-tuning](#pre-trained-models-fine-tuning)
    - [Transformer](#transformer)
  - [Data Utilization](#data-utilization)
    - [Weakly/Semi-supervised Learning](#weaklysemi-supervised-learning)
    - [Data Augmentation](#data-augmentation)
  - [Post-processing \& Inference](#post-processing--inference)
  - [DCASE Workshops \& Leaderboards](#dcase-workshops--leaderboards)
  - [License](#license)

## Introduction
This list is dedicated to researchers working on polyphonic SED with the DESED dataset. We categorize papers and resources strictly by system pipeline for easy navigation.

**Inclusion Criteria**:  
- Papers are primarily sourced from high-impact conferences and journals like ICASSP, Interspeech, and TASLP, but we also include influential works from other SED-related venues (e.g., DCASE Workshops, IEEE Signal Processing Letters).  
- Focus on papers published or accepted after 2022, with a few exceptional pre-2022 works for foundational contributions.
  
## Survey Papers
- **[Sound Event Detection: A Tutorial](https://ieeexplore.ieee.org/document/9524590)** (2021) - IEEE Signal Processing Magazine  

## Datasets & Benchmarks
| Dataset | Year | # Classes | Duration | Annotation Type | Link |
|---------|------|-----------|----------|-----------------|------|
| DESED   | 2019+ | 10        |  | Strong/Weak/Unlabel     | [Official](https://project.inria.fr/desed/) |
| MAESTRO-Real | 2023 | 10+       |  | Soft Label      | [Paper](https://arxiv.org/abs/2305.12345) |

## Frontend / Acoustic Features
Mostly Log-Mel

## Model Architectures

### CNN-based
- **[Frequency Dynamic Convolution](https://dcase.community/challenge2020/task-sound-event-detection-in-domestic-environments/results)** (Interspeech 2022)  - [Code](https://github.com/frednam93/FDY-SED)
- **[Multi-Dimensional Frequency Dynamic Convolution](https://ieeexplore.ieee.org/document/10096306/)** (ICASSP 2023)  
- **[Frequency Dynamic Convolution with Large Kernel Attention](https://arxiv.org/abs/2306.06461)** (arxiv 2023)  
- **[Frequency-aware Fourier Filter](https://ieeexplore.ieee.org/document/10889813)**(ICASSP 2025)
- **[Frequency & Channel Attention](https://dcase.community/documents/workshop2023/proceedings/DCASE2023Workshop_Nam_32.pdf)**(DCASE WorkShop 2023)
- **[Frequency-aware Convolution](https://link.springer.com/chapter/10.1007/978-981-96-2054-8_31)**(MMM 2025)
- **[Diversifying and Expanding Frequency-Adaptive Convolution](https://www.isca-archive.org/interspeech_2024/nam24_interspeech.html)**(Interspeech 2024)
- **[Dynamic Attention-Asymmetric Perceptron Network](https://ieeexplore.ieee.org/document/11340695)**(TASLP 2026)
- **[Multi-Dilated Frequency Dynamic Convolution](https://arxiv.org/abs/2406.13312)**(arxiv 2024)
- **[Temporal Attention Pooling](https://arxiv.org/abs/2504.12670)**(arxiv 2025)

### Pre-trained Models Fine-tuning
- **[AST-SED](https://ieeexplore.ieee.org/abstract/document/10096853)**(ICASSP 2023)
- **[ASiT-CRNN](https://www.sciencedirect.com/science/article/abs/pii/S1051200425000776)**(Digital Signal Processing, Accepted 2025)
- **[PaSST-SED](https://www.isca-archive.org/interspeech_2023/li23n_interspeech.html)**(Interspeech 2023)
- **[ATST-SED](https://ieeexplore.ieee.org/abstract/document/10446159)**(ICASSP 2024)
- **[MTDA-HSED](https://ieeexplore.ieee.org/document/10889194)**(ICASSP 2025)
- **[GE-FPT](https://ieeexplore.ieee.org/document/10889807)**(ICASSP 2025)
- **[ATST-Conformer Dual-Branch](https://www.isca-archive.org/interspeech_2025/dai25_interspeech.html)**(Interspeech 2025)

### Transformer



## Data Utilization

### Weakly/Semi-supervised Learning
- **[Random Consistency Training](https://www.isca-archive.org/interspeech_2022/shao22_interspeech.html)**(Interspeech 2022)
- **[Resolution Consistency Training](https://www.isca-archive.org/interspeech_2023/choi23b_interspeech.html)**(Interspeech 2023)
- **[Local and Global Consistency Regularization](https://ieeexplore.ieee.org/document/10446386/)**(ICASSP 2024)
- **[Confidence-aware Mean Teacher](https://www.sciencedirect.com/science/article/abs/pii/S1051200424004196)**(Digital Signal Processing, Available 2024)
- **[Dual Consistency Training](https://www.sciencedirect.com/science/article/abs/pii/S0925231226002778)**(Neurocomputing, Accepted 2026)

### Data Augmentation


## Post-processing & Inference
- **[Sound Event Bounding Boxes](https://www.isca-archive.org/interspeech_2024/ebbers24_interspeech.html)** (Interspeech 2024)  
 

## DCASE Workshops & Leaderboards
- [DESED Task Official Baselines](https://github.com/DCASE-REPO/DESED_task) - CRNN, Mean Teacher, etc. 

- [DCASE 2024 Task 4 Leaderboard](https://dcase.community/challenge2024/task-sound-event-detection-with-heterogeneous-training-dataset-and-potentially-missing-labels-results)  
- [DCASE 2023 TASK 4A Leaderboard](https://dcase.community/challenge2023/task-sound-event-detection-with-weak-labels-and-synthetic-soundscapes-results)

- [DCASE 2022 TASK 4 Leaderboard](https://dcase.community/challenge2022/task-sound-event-detection-in-domestic-environments-results)

## License
MIT License - See the [LICENSE](LICENSE) file for details.