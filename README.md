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
- `docs/`: Case study PDF.
- `requirements.txt`: Dependencies.

| Lifecycle Step | Tool(s) Used |
|----------------|--------------|
| Ingestion | pandas |
| Exploratory Analysis | matplotlib, seaborn, pandas |
| Transformation & Feature Engineering | sklearn.preprocessing (StandardScaler, LabelEncoder),<br>sklearn.decomposition (PCA) |
| Modeling | sklearn.cluster (KMeans, DBSCAN),<br>sklearn.ensemble (RandomForestClassifier),<br>sklearn.neighbors (NearestNeighbors) |
| Evaluation | sklearn.metrics (classification_report, confusion_matrix) |
| Storage | CSV (input/output files) |
| Visualization | matplotlib, seaborn |

## Installation and Setup
1. Clone the repo:
   ```bash
   git clone https://github.com/Rajvib-0/ott-viewer-dropoff-analysis
   
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

3. Run the notebook:
- Open [Notebook](ott_viewers_drop_off.ipynb) in Jupyter Notebook.
- Ensure the dataset path points to [Data](ott_viewer_dropoff_retention_us_v1.0.csv). 
   
