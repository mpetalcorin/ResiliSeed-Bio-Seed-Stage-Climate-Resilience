# Datasheet for Dataset

## Dataset name

**Synthetic Seed Resilience Dataset for ResiliSeed Bio Proof of Concept**

## Motivation

This dataset was created to support a **literature-benchmarked computational proof of concept** for seed-stage climate resilience. The goal was to test whether discovery, intervention ranking, and predictive modelling could be integrated into one coherent analytical framework before wet-lab and greenhouse validation.

The dataset was designed to represent how seed lots might behave under increasing stress complexity and under different seed-stage interventions.

## Dataset composition

The dataset contains row-level synthetic observations for seed lots from two crops:

- Tomato
- Pepper

Stress environments include:

- Control
- Heat
- Drought
- Combined heat + drought

Intervention classes include:

- None
- Hydropriming
- Melatonin
- Protein hydrolysate
- ResiliencePrimer

Each row represents one simulated seed-lot observation with associated physiological and performance measurements.

## Variables

The dataset includes variables such as:

- Crop
- Genotype class
- Stress condition
- Intervention
- Germination percentage
- Vigour index
- Electrolyte leakage percentage
- MDA
- Proline
- Catalase
- Root length
- Shoot length
- Recovery percentage
- Baseline seed attributes
- Composite resilience score, in derived analyses

## How the data were generated

The dataset is **synthetic**. Values were generated within biologically plausible ranges informed by published studies on:

- Seed physiology
- Seed priming
- Melatonin under drought stress
- Protein hydrolysates and biostimulants
- Oxidative damage and antioxidant responses
- Abiotic stress effects on germination and early seedling growth

The data were generated to preserve:

- Realistic stress-ranking behaviour
- Plausible intervention hierarchies
- Coherent trait correlations
- Observation-level variability

## What the dataset is not

This dataset is not:

- A measured wet-lab dataset
- A field dataset
- A greenhouse dataset
- A regulatory-grade dataset
- A commercial decision dataset

It should be treated as a **hypothesis-generating simulation dataset** only.

## Preprocessing

Categorical variables were encoded for modelling where needed. Numerical variables were used in descriptive summaries, correlation analysis, PCA, classification, and regression.

Derived outputs include:

- Summary tables by crop, stress, and intervention
- Heat + drought intervention rankings
- Correlation matrices
- PCA loadings
- Classifier metrics
- Regression metrics
- Commercial screening summaries

## Recommended uses

Appropriate uses include:

- Testing computational workflows
- Demonstrating proof-of-concept platform logic
- Building internal venture materials
- Planning wet-lab experiments
- Creating analysis pipelines for future real datasets

## Non-recommended uses

The dataset should not be used for:

- Real product claims
- Regulatory submissions
- Field recommendations
- Farmer guidance
- Breeding selection without validation
- Benchmarking real biological performance as if measured experimentally

## Distribution and access

This dataset is intended to live within the repository as a transparent research artifact supporting the notebook and manuscript outputs.

## Known limitations

- Synthetic rather than measured
- Limited to tomato and pepper
- Limited to a specific stress design
- Dependent on assumptions from benchmark literature
- Does not capture all sources of real-world seed-lot variability
- Does not include full formulation chemistry, storage effects, or field heterogeneity

## Future improvements

Future versions should incorporate:

- Real seed-lot measurements
- Additional crops
- More genotype diversity
- Storage-history metadata
- Greenhouse and field outcomes
- Real intervention dose-response data

## Relationship to figures and tables

This dataset underlies the principal analytical outputs in the repository, including:

- Stress-gradient plots
- Intervention ranking plots
- Leakage versus recovery relationships
- PCA visualisations
- Classifier performance
- Feature importance
- Recovery prediction
- Commercial prioritisation summaries

## Data stewardship statement

This dataset is provided to make the proof-of-concept workflow transparent and reproducible. It is best understood as a structured scaffold for future empirical work rather than as a substitute for experimental validation.
