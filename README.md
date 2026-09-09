Cardiovascular Risk Analysis Engine

A high-performance machine learning pipeline engineered to evaluate and classify cardiovascular disease (CVD) risk. This project integrates custom evolutionary algorithms, optimized spatial clustering, and probabilistic reasoning to handle complex, ambiguous clinical data.

## Architecture & Key Features

*   **Genetic Algorithm Feature Selection:** Built a custom GA from scratch (tournament selection, crossover, bit-flip mutation) to optimize feature subsets, maximizing cross-validation accuracy on a predictive logistic regression baseline.
*   **Optimized Unsupervised Clustering:** Partitioned a 20,000-record clinical dataset into actionable risk cohorts using K-Medoids (Manhattan distance) and Agglomerative Hierarchical clustering. 
*   **$O(N \log N)$ Complexity Reduction:** Optimized hierarchical clustering execution by generating a sparse K-Nearest Neighbors connectivity graph, successfully bypassing standard $O(N^3)$ dense matrix bottlenecks and reducing memory allocation overhead by 99.8%.
*   **Fuzzy Logic Inference System (FIS):** Designed an end-to-end inference engine that ingests raw physiological biometrics (Mean Arterial Pressure, BMI) alongside unsupervised cluster labels to dynamically compute clinical urgency scores.

## Tech Stack
*   **Languages:** Python 
*   **Libraries:** NumPy, Pandas, Scikit-Learn, skfuzzy, Matplotlib, Seaborn

## Dataset
Sourced from Kaggle, comprising ~20,000 sanitized patient records featuring demographic data, blood pressure metrics, and ordinal cholesterol/glucose levels.
