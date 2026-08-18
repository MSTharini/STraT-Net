# STraT-Bench

## Overview

STraT-Bench is a controlled synthetic longitudinal benchmark developed for
evaluating symptom-trajectory modelling in neurodegenerative disease
classification.

The benchmark was developed as part of the evaluation of STraT-Net
(Symptom Trajectory Transformer Network).

## Dataset Summary

STraT-Bench contains:

- 3,000 simulated patients
- 14,863 patient-year trajectory records
- 178,242 sentence-level clinical narrative records
- 3–7 annual encounters per patient
- Five neurodegenerative disease categories

The five disease categories are:

- Alzheimer's disease (AD)
- Parkinson's disease (PD)
- Lewy body dementia (LBD)
- Frontotemporal dementia (FTD)
- Multiple system atrophy (MSA)

## Synthetic Data Statement

STraT-Bench contains synthetic data generated for controlled methodological
evaluation.

It does not contain real patient records and should not be interpreted as a
clinically validated patient cohort.

The benchmark is designed to support reproducible evaluation of longitudinal
symptom-trajectory modelling rather than to reproduce the full heterogeneity
of real-world clinical practice.

## Data Generation

Synthetic longitudinal observations were generated using disease-specific
symptom propensities, a shared background profile, patient-specific random
effects, longitudinal noise, and longitudinal autocorrelation.

Structured symptom trajectories and corresponding clinical narratives were
generated from the same underlying synthetic visit state.

Explicit disease names were excluded from the generated clinical narratives
to reduce direct label leakage.

## Dataset Partitioning

Patients were partitioned at the patient level into:

- Training: 70% (2,100 patients)
- Validation: 15% (450 patients)
- Test: 15% (450 patients)

All observations belonging to an individual simulated patient were retained
within the same partition to prevent patient-level information leakage.

## Intended Use

STraT-Bench is intended for:

- Longitudinal machine-learning research
- Clinical NLP methodology development
- Symptom-trajectory modelling
- Temporal representation learning
- Controlled comparison of classification models
- Reproducibility studies

## Limitations

STraT-Bench does not reproduce the complete complexity of real clinical
populations, including comorbidities, missing data, irregular follow-up,
documentation variability, and broader clinical heterogeneity.

Results obtained using STraT-Bench should therefore be interpreted as
methodological or proof-of-concept evidence rather than evidence of
real-world clinical diagnostic performance.

## Clinical Disclaimer

STraT-Bench and STraT-Net are provided for research purposes only.

They are not validated medical devices and are not intended for clinical
diagnosis, treatment decisions, or direct patient-care applications.

## Citation

If you use STraT-Bench in your research, please cite the associated STraT-Net
publication and software repository.

Full publication citation details will be added following publication.
