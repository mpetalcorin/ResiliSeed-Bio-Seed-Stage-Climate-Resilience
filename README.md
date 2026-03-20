# ResiliSeed Bio Seed Stage Climate Resilience

A literature-benchmarked computational proof of concept for **seed-stage climate resilience** under **combined heat and drought stress**, integrating **seed physiology**, **intervention ranking**, and **machine learning prediction**.
<img width="1438" height="1062" alt="ResiliSeed Bio" src="https://github.com/user-attachments/assets/40c5b1c6-c97b-418d-8943-6c47408b8fab" />

## Overview

This repository contains a synthetic, literature-informed analysis framework built around the **ResiliSeed Bio** concept. The project explores whether seed-stage resilience can be modelled as an integrated platform with three connected components:

1. **Discovery engine** for identifying resilience-associated biomarkers.
2. **Intervention engine** for ranking seed-stage treatments.
3. **Prediction engine** for classifying and forecasting resilience outcomes.

The analysis focuses on **tomato** and **pepper** seed lots across four environmental conditions:

- Control
- Heat
- Drought
- Combined heat + drought

Candidate seed-stage interventions include:

- Hydropriming
- Melatonin
- Protein hydrolysate
- ResiliencePrimer, a hypothetical composite formulation

## Key questions

This repository addresses five practical questions:

- How strongly does germination decline as stress complexity increases?
- Which interventions best improve recovery under combined heat + drought stress?
- Which physiological variables are most associated with resilience?
- Can high-resilience outcomes be predicted using machine learning?
- Which intervention-crop combinations appear most attractive for pilot-partner prioritisation?

## Main outputs

The repository includes:

- An executed notebook
- A synthetic seed resilience dataset
- Summary tables
- Figures
- A README, model card, and data sheet

## Headline findings

- Untreated seed lots showed progressive declines in germination, vigour, and recovery as stress complexity increased.
- Combined heat + drought imposed the strongest stress penalty.
- Intervention-treated seed lots outperformed untreated controls under compound stress.
- **ResiliencePrimer** ranked highest overall, followed by **melatonin** and **protein hydrolysate**.
- Lower **electrolyte leakage** and lower **MDA** were associated with improved recovery.
- The classifier achieved strong discrimination of high-resilience outcomes, with an **ROC-AUC of 0.95**.
- Recovery could also be predicted quantitatively using regression.
- Germination, electrolyte leakage, MDA, catalase, and vigour were the strongest predictive features.

## Repository structure

```text
ResiliSeed_Bio_proof_of_concept.ipynb
synthetic_seed_resilience_dataset.csv
summary_by_crop_stress_intervention.csv
heat_drought_intervention_ranking.csv
Table_*.csv
Figure_*.png
README.md
modelcard.md
datasheet.md
```

## Methods summary

The project uses a **synthetic dataset** generated within biologically plausible ranges informed by peer-reviewed studies on:

- Seed physiology
- Priming
- Melatonin
- Protein hydrolysates
- Oxidative stress
- Abiotic stress responses

Measured and derived variables include:

- Germination percentage
- Vigour index
- Electrolyte leakage
- Malondialdehyde, MDA
- Proline
- Catalase
- Root length
- Shoot length
- Recovery percentage
- Composite resilience score

Analytical methods include:

- Descriptive summaries
- Correlation analysis
- Principal component analysis, PCA
- Classification modelling
- Regression modelling
- Permutation feature importance
- Commercial screening for pilot-partner prioritisation

## Intended use

This repository is intended for:

- Proof-of-concept exploration
- Venture framing
- Internal R&D planning
- Seed-stage resilience hypothesis generation
- Pitching an early platform concept
- Guiding future wet-lab and greenhouse experiments

## Important limitation

This repository does **not** provide experimental confirmation. The dataset is **synthetic and hypothesis-generating**, not wet-lab or field validated. Numerical outputs should therefore be interpreted as **literature-benchmarked scenario analysis** rather than definitive agronomic performance claims.

## Future directions

Planned next steps include:

- Controlled germination assays under heat + drought
- Real seed-lot validation in tomato and pepper
- Biomarker measurement in wet-lab experiments
- Greenhouse validation
- Expanded intervention testing
- Crop-specific optimisation
- Partner-facing pilot studies

## Citation

If you use this repository, cite it as:

**Petalcorin, M. I. R.** (2026) ResiliSeed Bio: Proof of concept for seed-stage climate resilience under combined heat and drought stress. https://github.com/mpetalcorin/ResiliSeed-Bio-Seed-Stage-Climate-Resilience

## Contact

**Mark Ihrwell R. Petalcorin, PhD**  
Scientist in plant breeding, seed technology, molecular biology, biochemistry, and AI-enabled scientific research.

