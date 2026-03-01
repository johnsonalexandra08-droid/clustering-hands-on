# M7: Clustering with K-Means and DBSCAN

**Course:** Introduction to Machine Learning  
**Instructor:** Becky Deitenbeck  
**Student:** Hannah Johnson  
**Date:** March 3, 2026  

---

## Assignment Overview

This assignment applies unsupervised learning techniques to the Wine dataset using Python and scikit-learn. Both K-Means and DBSCAN clustering algorithms are implemented, compared, and interpreted. Results are visualized and documented using GitHub.

---

## Instructions

1. **Data Exploration** — Load the Wine dataset, display summary statistics, and visualize feature distributions.
2. **K-Means Clustering** — Scale features, apply K-Means for K=2–6, use the Elbow method to select the optimal K, and visualize clusters.
3. **DBSCAN Clustering** — Apply DBSCAN with varied `eps` and `min_samples`, visualize results including noise points.
4. **Reflection** — Discuss real-world applications and ethical considerations of clustering.

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/clustering-hands-on.git
   cd clustering-hands-on
   ```

2. Install requirements:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```

3. Open the notebook:
   ```bash
   jupyter notebook M7_Clustering_KMeans_DBSCAN.ipynb
   ```
   Or upload to **Google Colab** and run cell-by-cell.

---

## Dataset

- **Name:** Wine Dataset
- **Source:** `sklearn.datasets.load_wine()`
- **Samples:** 178 wine samples from 3 cultivars
- **Features:** 13 chemical measurements (alcohol, malic acid, ash, etc.)
- **Use:** Unsupervised clustering — true labels used only for evaluation, not training

---

## Files in This Repository

| File | Description |
|------|-------------|
| `README.md` | Project overview and instructions |
| `M7_Clustering_KMeans_DBSCAN.ipynb` | Main Jupyter Notebook with all code and analysis |

---

## Key Findings

- K-Means with **K=3** best matches the Wine dataset's known structure, confirmed by the Elbow method and Adjusted Rand Index.
- DBSCAN identified core clusters but required careful tuning — the Wine dataset's high dimensionality and uniform density make it less ideal for DBSCAN than K-Means.
- Feature scaling is critical for both algorithms to perform correctly.

---

## Submission

- Push completed notebook and README to this repository.
- Submit the repository link in Canvas.
