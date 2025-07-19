# 🤖 CodeBERT vs CodeT5+ – Code Similarity & Clustering using Transformers

This project presents a comparative analysis of **CodeBERT** and **CodeT5+** for evaluating code similarity and clustering programming solutions. It focuses on unsupervised learning, leveraging deep code embeddings and dimensionality reduction for visual and quantitative analysis.

---

## 🧠 Objectives

- Generate vector embeddings from code using CodeBERT and CodeT5+
- Apply clustering algorithms (KMeans, DBSCAN) on embeddings
- Visualize clusters using UMAP/t-SNE
- Evaluate clustering quality (Silhouette Score, Davies-Bouldin Index)
- Compare model performance on different programming styles and structures

---

## 🚀 Workflow Overview

1. Collect coding solutions from programming platforms (e.g., Codeforces, LeetCode)
2. Clean and tokenize the code
3. Generate embeddings using:
   - 🧠 CodeBERT (via `microsoft/codebert-base`)
   - 🧠 CodeT5+ (via `Salesforce/codet5p-220m`)
4. Cluster embeddings using DBSCAN / KMeans
5. Reduce dimensions using UMAP / t-SNE for 2D visualization
6. Evaluate and compare clustering effectiveness

---

## 📊 Results Summary

| Metric              | CodeBERT   | CodeT5+    |
|---------------------|------------|------------|
| Silhouette Score    | 0.41       | 0.58       |
| Davies-Bouldin      | 0.88       | 0.61       |
| Visual Separation   | Moderate   | High       |
| Embedding Density   | Sparse     | Compact    |

✅ **CodeT5+** demonstrated better clustering performance and cleaner separation for structurally similar code.

---

---

## 🧰 Tech Stack

| Component            | Libraries/Models                              |
|----------------------|-----------------------------------------------|
| Code Embedding       | CodeBERT (HuggingFace), CodeT5+               |
| Clustering           | Scikit-learn (DBSCAN, KMeans)                 |
| Dimensionality Reduction | UMAP, t-SNE                            |
| Visualization        | Matplotlib, Seaborn, Plotly                   |
| Evaluation Metrics   | Silhouette Score, Davies-Bouldin Index        |
| Language             | Python (PyTorch, Transformers, NumPy, etc.)   |

---

## 💡 Research Use Cases

- Code plagiarism detection  
- Code submission clustering for educators  
- Detecting stylistic patterns in developer behavior  
- Building AI-assisted feedback tools for code

---
