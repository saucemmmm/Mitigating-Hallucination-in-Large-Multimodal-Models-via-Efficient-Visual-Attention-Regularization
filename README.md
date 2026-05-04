# Mitigating Hallucination in Large Multimodal Models via Efficient Visual Attention Regularization

This repository contains the code, datasets, and findings for the CISC874 course project. The primary goal of this project is to explore and implement methods for mitigating hallucinations in Large Multimodal Models (LMMs) using an efficient visual attention regularization technique.

## Project Report

For a detailed explanation of the methodology, theoretical background, and a comprehensive analysis of our findings, please refer to the project report:
**[`CISC874___Project_Report.pdf`](./CISC874___Project_Report.pdf)**

## Experiments and Reproducibility

To ensure full reproducibility of the experiments discussed in the project report, this repository includes the Jupyter notebooks and necessary benchmark datasets used during our evaluation. 

### Notebooks
- **`CISC874_Baseline.ipynb`**: Contains the baseline implementation and evaluation code used to measure initial model hallucinations before any interventions.
- **`CISC874Projec.ipynb`**: Contains the main implementation of our visual attention regularization approach and the experimental setup to evaluate its effectiveness against the baselines.

### Datasets and Results
The provided `.zip` files contain the datasets, images, and raw experimental results associated with the standard multimodal benchmarks we used. You will need these to reproduce the project results:
- **`MME.zip`**: Data and resources related to the MME benchmark.
- **`MMVP.zip`**: Data and resources related to the MMVP benchmark.
- **`POPE.zip`**: Data and resources related to the POPE (Polling-based Object Probing Evaluation) benchmark.

## How to Use
1. Unzip the benchmark archive files (`MME.zip`, `MMVP.zip`, `POPE.zip`) into your working directory as required by the notebooks.
2. Run `CISC874_Baseline.ipynb` to evaluate the baseline hallucination metrics.
3. Run `CISC874Projec.ipynb` to apply the efficient visual attention regularization and observe the mitigation results as detailed in the report.