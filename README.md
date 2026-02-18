# Viewer Retention in OTT Platforms: Diagnosing Engagement Pattern

## Overview
This capstone project for Winter Consulting 2025 (Consulting & Analytics Club, IIT Guwahati) analyzes viewer drop-off in OTT platforms using data from over 33,000 episodes. The goal is to identify key drivers of retention, segment content via clustering, and propose ML-driven interventions to reduce drop-off rates.

**Key Objectives**:
- Diagnose high drop-off in genres like Drama and Mystery.
- Use correlation, clustering, and predictive modeling.
- Recommend strategies.

**Tech Stack**: Python, Pandas, Scikit-learn, Matplotlib/Seaborn.

## Key Findings
- Strong negative correlation (-0.96) between average watch percentage and drop-off probability.
- High-risk genres: Drama, Mystery, Western (higher drop-off).
- Optimal pacing score: 4-6; High cognitive load (score 9) leads to 79.6% drop-off.
- Clusters: 0 (Best: 0% drop-off), 1&2 (Balanced: ~65% watch), 3 (Worst: 55.4% drop-off).
- ML Model: 85% accuracy in predicting drop-off using features like cognitive load, hook strength, and pacing.

For full details, see [RAJVI_case_study_2.pdf](docs/RAJVI_case_study_2.pdf).

## Repository Structure
- `notebooks/`: Main analysis in Jupyter notebook.
- `data/`: Dataset (CSV).
- `docs/`: Case study PDF and presentation slides.
- `results/`: Output CSV with clusters and plots.
- `requirements.txt`: Dependencies.

## Installation and Setup
1. Clone the repo:
