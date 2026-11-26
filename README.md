# Discovering Unusual Astronomical Objects Using Multimodal Neural Anomaly Detection

An astronomy and machine learning research project exploring unsupervised anomaly detection in Gaia DR3 data.

## Overview

This project investigates whether multimodal unsupervised learning can identify potentially unusual astronomical objects by combining astrometric, photometric, and temporal features.

The workflow includes data acquisition, data quality assessment, feature engineering, anomaly detection, neural representation learning, multimodal fusion, cross-matching validation, and candidate analysis.

## Research Objectives

- Explore Gaia DR3 data for potentially unusual astronomical sources.
- Develop and evaluate unsupervised anomaly detection approaches.
- Investigate the contribution of individual feature groups.
- Combine astrometric, photometric, and temporal information.
- Prioritise candidate objects for further astronomical investigation.

## Methodology

1. Astronomy background and data acquisition.
2. Data quality assessment and cleaning.
3. Astrophysical feature engineering.
4. Baseline anomaly detection.
5. Autoencoder-based representation learning.
6. Temporal feature analysis.
7. Multimodal feature fusion.
8. SIMBAD cross-matching and validation.
9. Visualisation and candidate analysis.
10. Model export and final candidate catalogue.

## Repository Structure

    astronomy-project/
    ├── data/
    │   ├── raw/
    │   ├── intermediate/
    │   └── processed/
    ├── notebooks/
    ├── results/
    │   ├── candidates/
    │   ├── evaluation/
    │   └── figures/
    ├── src/
    ├── requirements.txt
    ├── .gitignore
    └── README.md

## Notebooks

The numbered notebooks follow the research workflow, from astronomy fundamentals and data acquisition through to model export and candidate analysis.

## Data

The project uses Gaia DR3 catalogue measurements and derived astrophysical features.

**Important:** The temporal features were generated synthetically for the initial sample. They should not be interpreted as observed Gaia epoch photometry or real measured light curves.

- Gaia DR3: https://www.cosmos.esa.int/web/gaia/dr3
- SIMBAD: https://simbad.cds.unistra.fr/

## Installation

Clone the repository:

    git clone <YOUR-REPOSITORY-URL>
    cd astronomy-project

Create and activate a virtual environment:

    python3 -m venv .venv
    source .venv/bin/activate

Install dependencies:

    pip install --upgrade pip
    pip install -r requirements.txt

Launch Jupyter:

    jupyter notebook

## Results

The results directory contains candidate catalogues, evaluation outputs, diagnostic files, and visualisations produced during the project.

## Limitations

- Unsupervised anomaly scores identify unusual patterns, not confirmed astronomical discoveries.
- Candidate objects require further scientific investigation.
- Synthetic temporal features are not equivalent to real observational light curves.
- Cross-matching provides supporting context and does not independently establish that an object is anomalous.

## Reproducibility

The numbered notebooks document the analysis workflow. Results may vary depending on package versions, random seeds, and computational environment.

## Acknowledgements

This research makes use of data from the European Space Agency (ESA) Gaia mission and the SIMBAD astronomical database.

## License

A license will be added after the repository's publication terms are finalised.
