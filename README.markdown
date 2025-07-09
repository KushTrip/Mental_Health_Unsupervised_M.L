# Unsupervised Machine Learning: Mental Health in Tech Jobs

## Project Overview
This repository contains the code and resources for a case study on applying unsupervised machine learning to analyze mental health trends among tech employees, using the 2016 OSMI Mental Health in Tech Survey dataset. The project clusters employees based on mental health and workplace experiences, reduces data dimensionality, and provides actionable HR insights.

**Course:** Machine Learning – Unsupervised Learning (DLBDSMLUSL01)  
**Author:** Kush Tripathi  
**Date:** 09/07/2025

---

## Table of Contents
- [Prerequisites](#prerequisites)
- [Dataset](#dataset)
- [Running the Code](#running-the-code)
- [Project Structure](#project-structure)
- [Results](#results)
- [License](#license)

---

## Prerequisites
To run this project, 
Either create an account in GoogleCollab and download the ipynb file and open it in Google collab
Or
If you want torun it locally, ensure you have the following installed:
- Python 3.8 or higher
- pip (Python package manager)
- Jupyter Notebook or any Python IDE (e.g., VS Code, PyCharm)
- Required Python libraries :
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn

---

## Dataset
The project uses the **2016 OSMI Mental Health in Tech Survey** dataset, available on Kaggle:  
[OSMI Mental Health in Tech Survey](https://www.kaggle.com/osmi/mental-health-in-tech-survey)

### Steps to Load the Dataset
1. Download the `mental-heath-in-tech-2016_20161114.csv` dataset from this repository or the Kaggle link above.
2. Note: Ensure the dataset is successfully loaded before running the notebook.


## Running the Code
1. **Open the Jupyter Notebook**  
   Open Google Collab website OR Launch Jupyter Notebook 

2. **Run the Main Notebook**  
   Open `mental_health_case_study_KushTrip.ipynb` and execute all cells sequentially. The notebook includes:
   - Data loading and preprocessing
   - Feature engineering
   - Dimensionality reduction (PCA, MDS)
   - Clustering (K-Means, GMM, Hierarchical)
   - Visualization (PCA scatterplot, heatmap, dendrogram)
   - Evaluation (Elbow method, Silhouette score)

3. **Expected Output**  
   - Visualizations saved in the `outputs/` folder (e.g., `pca_scatterplot.png`, `heatmap.png`).
   - Cluster analysis results printed in the notebook.
---

## Project Structure
```
├── data/
│   └── mental-heath-in-tech-2016_20161114.csv              # Dataset 
├── notebooks/
│   └── mental_health_case_study_KushTrip.ipynb             # Main IPYNB file with all code
├── outputs/
│   └── [visualizations]       # Generated plots, diagrams, graphs (e.g., elbow method.png)
└── README.md                  # This file
```

---

## Results
The analysis identifies two employee clusters:
- **Cluster 0:** Employees with high mental health interference and low workplace support, often in smaller companies.
- **Cluster 1:** Employees with lower mental health issues and better support, typically in larger firms.

Key visualizations include:
- PCA scatterplot showing cluster separation.
- Heatmap highlighting correlations between mental health interference and support.

**HR Insights:**
- Targeted interventions (e.g., counseling, flexible hours) for Cluster 0.
- Scale successful policies from Cluster 1 across organizations.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
