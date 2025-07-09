# Unsupervised Machine Learning: Mental Health in Tech Jobs

## Project Overview
This repository contains the code and resources for a case study on applying unsupervised machine learning to analyze mental health trends among tech employees, using the 2016 OSMI Mental Health in Tech Survey dataset. The project clusters employees based on mental health and workplace experiences, reduces data dimensionality, and provides actionable HR insights.

**Course:** Machine Learning – Unsupervised Learning (DLBDSMLUSL01)  
**Author:** [Your Name]  
**Date:** [Insert Date]

---

## Table of Contents
- [Prerequisites](#prerequisites)
- [Dataset](#dataset)
- [Installation](#installation)
- [Running the Code](#running-the-code)
- [Project Structure](#project-structure)
- [Results](#results)
- [License](#license)

---

## Prerequisites
To run this project, ensure you have the following installed:
- Python 3.8 or higher
- pip (Python package manager)
- Jupyter Notebook or any Python IDE (e.g., VS Code, PyCharm)
- Required Python libraries (listed in `requirements.txt`):
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
1. Download the dataset (`survey.csv`) from the Kaggle link above.
2. Place the `survey.csv` file in the `data/` folder of this repository.
3. Ensure the file path in the code (`notebooks/main.ipynb`) points to `data/survey.csv`.

---

## Installation
Follow these steps to set up the project environment:

1. **Clone the Repository**  
   ```bash
   git clone [your-repository-url]
   cd [repository-name]
   ```

2. **Create a Virtual Environment**  
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

4. **Verify Setup**  
   Ensure Jupyter Notebook is installed:  
   ```bash
   jupyter notebook
   ```

---

## Running the Code
1. **Open the Jupyter Notebook**  
   Launch Jupyter Notebook and navigate to the `notebooks/` folder:  
   ```bash
   jupyter notebook
   ```

2. **Run the Main Notebook**  
   Open `notebooks/main.ipynb` and execute all cells sequentially. The notebook includes:
   - Data loading and preprocessing
   - Feature engineering
   - Dimensionality reduction (PCA, MDS)
   - Clustering (K-Means, GMM, Hierarchical)
   - Visualization (PCA scatterplot, heatmap, dendrogram)
   - Evaluation (Elbow method, Silhouette score)

3. **Expected Output**  
   - Visualizations saved in the `outputs/` folder (e.g., `pca_scatterplot.png`, `heatmap.png`).
   - Cluster analysis results printed in the notebook.

**Note:** Ensure the dataset (`survey.csv`) is in the `data/` folder before running the notebook.

---

## Project Structure
```
├── data/
│   └── survey.csv              # Dataset (place here after downloading)
├── notebooks/
│   └── main.ipynb             # Main Jupyter Notebook with all code
├── outputs/
│   └── [visualizations]       # Generated plots (e.g., pca_scatterplot.png)
├── requirements.txt           # List of Python dependencies
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