# 📊 Data Version Control (DVC)

[DVC (Data Version Control)](https://dvc.org/)) is an **open-source** version control system specifically designed for machine learning projects.

## 🚀 Why DVC?

While **Git** is the industry standard for versioning source code, it is not built to handle large files. **DVC** bridges this gap:

*   **Git is for Code:** Git handles small text files efficiently but slows down significantly with large binaries.
*   **DVC is for Data:** It allows you to version control large datasets (CSV, images, databases), ML models, and pipeline outputs without bloating your Git repository.

## 🛠️ Key Capabilities

*   **Large File Management:** Version control files that are too big for Git by storing them in external storage (S3, GCP, Azure, or local remotes).
*   **Pipeline Tracking:** Manage and reproduce multi-stage workflows, including data cleaning, training, and evaluation.
*   **Metric Logging:** Version your experiment results and performance metrics alongside your data.

## 💡 How it Works

1.  **Track:** You tell DVC to track a large file (e.g., `dataset.csv`).
2.  **Pointer:** DVC creates a lightweight `.dvc` file (a pointer).
3.  **Sync:** You commit the small `.dvc` file to **Git**, while the actual heavy data is pushed to your **DVC Remote Storage**.

---
*For more information on how to get started, check out the [Official DVC Documentation](https://dvc.org/).*
