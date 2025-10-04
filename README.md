# Assignment 5 — Visualizing Data Veracity Challenges in Multi-Label Classification  

**Name:** Priyanshu Verma  
**Roll no:** CH22B087  
**Date:** 04-10-2025  

---

## Project Overview  

This notebook explores **data veracity challenges in multi-label classification** using the **Yeast dataset**. The dataset represents gene expression profiles with **103 features** and **14 functional categories** as labels. The focus of this assignment is on identifying **noisy or ambiguous labels, outliers, and hard-to-learn samples** that make classification difficult.  

To achieve this, two advanced **non-linear dimensionality reduction techniques** — **t-SNE** and **Isomap** — were applied to project the high-dimensional feature space into two dimensions. Visualizations of these embeddings were then analyzed to highlight regions where data quality issues arise, offering insights into the limitations faced by classifiers when dealing with biological data.  

The main deliverable is a Jupyter Notebook (`DA5401_Assignment_5.ipynb`) that includes preprocessing, dimensionality reduction, visualization, and interpretation of the results.  

---

## Files in this Repository  

- `DA5401_Assignment_5.ipynb` — main notebook (completed assignment).
- `yeast.arff` — the dataset.  
- `README.md` — this file.  

---

## Notebook Structure  

The notebook is structured into the following logical sections:  

1. **Assignment Description** — Overview of the dataset and objectives.  
2. **Part A: Preprocessing and Initial Setup** — Data loading, scaling, and label selection for visualization.  
3. **Part B: t-SNE and Veracity Inspection** — Applying t-SNE with varying perplexities, visualization, and identification of noisy labels, outliers, and hard-to-learn samples.  
4. **Part C: Isomap and Manifold Learning** — Applying Isomap, visualizing embeddings, and comparing global vs. local structure preservation.  
5. **Comparison & Conclusion** — Analyzing how t-SNE and Isomap reveal different aspects of the dataset’s manifold and data veracity issues.  Final insights on visualization, manifold complexity, and implications for classification.  

---

## Results  

- **t-SNE Visualization:**  
  - Clear local clusters for frequent categories.  
  - Revealed ambiguous samples embedded in different class clusters.  
  - Outliers appeared as isolated points or small clusters.  

- **Isomap Visualization:**  
  - Preserved more global structure.  
  - Suggested the dataset lies on a **complex, curved manifold**, reflecting the difficulty of learning functional categories.  

 Overall, **t-SNE** was more effective at detecting local ambiguities and hard-to-learn samples, while **Isomap** provided insights into the global manifold structure.  

---

## Requirements  

Recommended Python environment:  

- Python 3.8+ (3.9/3.10 recommended)  
- JupyterLab or Jupyter Notebook (or Google Colab)  

### Python Packages  

```bash
pip install pandas numpy scikit-learn seaborn matplotlib
