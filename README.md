#Project_1

# PageRank Implementation

This repository contains implementations of the **PageRank algorithm**.

The goal of this project is to compute and compare the **PageRank scores** for nodes in the **Stanford-Berkeley Web Graph dataset**. The implementation is done in three stages:

1. **Custom PageRank (Power Iteration)**  
   - Implemented from scratch using the Power Iteration method.  
   - Produces PageRank scores and reports the top-ranked pages by ID.  

2. **Eigenvector-based PageRank**  
   - Uses `numpy.linalg.eig` to compute eigenvectors of the transition matrix.  
   - Compares the results and runtime with the Power Iteration method.  

3. **NetworkX Comparison**  
   - Uses built-in functions from `networkx` to compute PageRank.  
   - Compares and interprets differences with the custom implementation.  

Additionally, the effect of **varying the damping factor α** is explored and analyzed to study its influence on the final ranking.

## Dataset
We use the [Stanford-Berkeley Web Graph dataset](https://www.kaggle.com/datasets/wolfram77/graphs-snap-web/data), but only process the **first 1000×1000 submatrix** (`Data[:1000, :1000]`) due to its large size.  

## Environment
The code can be executed on **Google Colab** or locally with Python. If additional compute resources are required, Colab is recommended.  

## Key Learnings
- Understanding of **Markov Chains** and **Random Walks** as the foundation of PageRank.  
- Hands-on experience with iterative methods (Power Iteration) vs. direct eigenvalue computation.  
- Insights into how damping factor tuning changes the ranking distribution. 
--------------------------------------------------------------------------------------------------------------------
#Project_2
# QR Decomposition – Least Squares Classification (EMNIST Letters)

This repository contains an implementation of **QR decomposition–based least squares classification**.

The project focuses on solving a **multi-class classification problem** using **QR decomposition** and updating techniques for least-squares solutions.

### 1. Initial Model Training
- Load the **EMNIST Letters** dataset.  
- Select **200 training samples per class** and form the training matrix.  
- Solve the least squares classification problem:
  - Compute the **QR decomposition** of the training matrix (using Householder reflections).
  - Solve for the weight matrix using back-substitution.
- Evaluate model accuracy on a separate **test set**.

### 2. QR Updating
- Introduce **20 new samples per class** (simulating incremental data).
- Update the QR decomposition efficiently **without recomputing from scratch**, using QR updating techniques.
- Solve the updated least-squares system and re-evaluate performance.
- Compare accuracy **before and after updating**.


## Key Concepts
- **QR decomposition** with Householder reflections.
- **Incremental QR updating** for efficient retraining.
- **Least-squares classification** for multi-class problems.
- Performance comparison between initial model and updated model.

## Environment
This project can be run locally or in **Google Colab** using:
- `numpy` (linear algebra operations)
- `scipy` (optional for QR decomposition)
- `matplotlib` (visualization of results)
---------------------------------------------------------------------------------------------------------------------
#Project_3

---------------------------------------------------------------------------------------------------------------------#Project_4
---------------------------------------------------------------------------------------------------------------------#Final_Project
