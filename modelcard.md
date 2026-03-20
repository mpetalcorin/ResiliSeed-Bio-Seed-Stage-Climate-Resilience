# Model Card

## Model name

**ResiliSeed Bio Prediction Engine**

## Model version

Version 1.0, proof-of-concept

## Model type

This repository contains two predictive model types:

1. **Binary classifier** for identifying **high-resilience** versus **lower-resilience** seed outcomes under combined heat + drought stress.
2. **Regression model** for predicting continuous **recovery percentage** under combined heat + drought stress.

## Intended use

The models are intended to support a **seed-stage resilience platform** by helping answer two practical questions:

- Which seed lots are likely to show high resilience under compound stress?
- What level of post-stress recovery is expected for a given seed lot and intervention combination?

This is designed for:

- Internal research and development
- Hypothesis generation
- Biomarker prioritisation
- Early-stage platform design
- Venture and partner discussion support

## Out-of-scope use

These models are **not** intended for:

- Direct agronomic recommendations in commercial farming
- Regulatory decision-making
- Breeding decisions without real experimental validation
- Clinical, medical, or safety-critical contexts
- Claims of field efficacy without wet-lab, greenhouse, and field testing

## Training data

The models were trained on a **synthetic, literature-benchmarked dataset** representing tomato and pepper seed lots under:

- Control
- Heat
- Drought
- Combined heat + drought

Intervention classes included:

- None
- Hydropriming
- Melatonin
- Protein hydrolysate
- ResiliencePrimer

Input features included physiological, performance, and metadata variables such as:

- Germination percentage
- Vigour index
- Electrolyte leakage
- MDA
- Proline
- Catalase
- Root length
- Shoot length
- Baseline seed features
- Crop identity
- Genotype class
- Intervention class

## Target variables

### Classifier target
High-resilience outcome under combined heat + drought stress.

### Regression target
Recovery percentage under combined heat + drought stress.

## Performance summary

### Classification
- ROC-AUC: **0.95**

Additional metrics are provided in `Table_6_classifier_metrics.csv` and `Table_7_confusion_matrix.csv`.

### Regression
Regression performance metrics are provided in `Table_9_regression_metrics.csv`.

## Key predictive features

Top predictive variables included:

- Germination percentage
- Electrolyte leakage
- MDA
- Catalase
- Vigour index

These features are biologically interpretable and align with known mechanisms of seed injury and stress recovery.

## Biological rationale

The model is grounded in the idea that seed-stage resilience under compound stress depends on coordinated biological processes including:

- Membrane integrity
- Oxidative stress buffering
- Antioxidant capacity
- Seedling vigour
- Post-stress recovery ability

The strong contribution of leakage, MDA, catalase, and vigour supports the mechanistic coherence of the prediction framework.

## Limitations

This model has important limitations:

- It is trained on **synthetic data**, not experimental data.
- The data are literature-benchmarked but do not represent a real seed-lot collection.
- The performance metrics reflect proof-of-concept conditions only.
- The model may not generalise to real commercial seed lots, additional crops, or other stress combinations.
- Threshold definitions for high resilience are internal to this proof of concept.

## Ethical and practical considerations

Because the model is synthetic and exploratory, it should not be used to overstate readiness or product efficacy. Its main value lies in shaping future experiments and guiding platform design.

Any real-world deployment should include:

- Independent wet-lab validation
- Greenhouse validation
- Field testing
- Crop-specific calibration
- Batch and seed-lot reproducibility checks

## Recommended next steps

To improve the model:

- Replace synthetic inputs with measured seed-lot data
- Add more crops and genotype diversity
- Include real storage-history variables
- Evaluate external validation performance
- Compare alternative modelling frameworks
- Build intervention recommendation logic from real treatment-response data

## Maintenance

This proof-of-concept model should be treated as a **research prototype**. Any future versions should document:

- Dataset changes
- Feature changes
- Threshold changes
- Retraining procedures
- Validation metrics on real-world data
