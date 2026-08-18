# STraT-Net

Official implementation of **STraT-Net (Symptom Trajectory Transformer Network)**,
a longitudinal artificial intelligence framework for modelling symptom evolution
across sequential clinical narratives for neurodegenerative disease classification.

## Overview

STraT-Net combines contextual clinical representations, biomedical concept
normalization, longitudinal symptom trajectory construction, Transformer-based
temporal reasoning, and gated temporal attention.

The framework is designed to model information distributed across successive
clinical encounters rather than treating individual visits independently.

## Target Disease Categories

The framework is evaluated across five neurodegenerative disease categories:

- Alzheimer's disease (AD)
- Parkinson's disease (PD)
- Lewy body dementia (LBD)
- Frontotemporal dementia (FTD)
- Multiple system atrophy (MSA)

## STraT-Bench

STraT-Bench is a controlled synthetic longitudinal benchmark developed for
evaluating longitudinal symptom-trajectory modelling.

It contains:

- 3,000 simulated patients
- 14,863 patient-year trajectory records
- 3–7 annual encounters per patient
- Five neurodegenerative disease categories

**Important:** STraT-Bench is a synthetic research benchmark and does not
represent a clinically validated patient cohort. Results obtained using this
benchmark should not be interpreted as evidence of real-world clinical
diagnostic performance.

## Model

STraT-Net integrates:

1. Contextual clinical narrative representation
2. Biomedical concept normalization
3. Longitudinal symptom trajectory construction
4. Transformer-based temporal reasoning
5. Gated temporal attention
6. Multi-class neurodegenerative disease classification

The temporal attention mechanism provides visit-level importance estimates
for examining the relative contribution of encounters to model predictions.
These importance scores should not be interpreted as causal clinical
explanations.

## Baseline Models

STraT-Net is compared against:

- TF-IDF + SVM
- TextCNN
- BiLSTM
- ClinicalBERT

## Repository Structure

```text
STraT-Net/
├── README.md
├── LICENSE
├── requirements.txt
├── CITATION.cff
├── configs/
├── data/
├── src/
├── scripts/
├── baselines/
├── results/
└── notebooks/
