# Mitigating Hallucination in Large Multimodal Models via Efficient Visual Attention Regularization

This repository contains the code, datasets, and findings for the CISC874 course project. The primary goal of this project is to explore and implement methods for mitigating hallucinations in Large Multimodal Models (LMMs) using an efficient visual attention regularization technique.

## Project Report

For a detailed explanation of the methodology, theoretical background, and a comprehensive analysis of our findings, please refer to the project report:
**[`CISC874___Project_Report.pdf`](./CISC874___Project_Report.pdf)**

## Experiments and Reproducibility

To ensure full reproducibility of the experiments discussed in the project report, this repository includes the Jupyter notebooks and necessary benchmark datasets used during our evaluation. We have added the 3 correct `.ipynb` files, each with the code used to get the results.

### Notebooks
- **Baseline Model**: Note the baseline model does not use any visual hallucination mitigation, we just running the image text pairs on the LLaVA-1.5-7B model.
- **Reproduce VCD**: The reproduce VCD is used to replicate the results found in the paper: [@seilk/VisAttnSink](https://github.com/seilk/VisAttnSink) (although we use a small subset of data than in the paper).
- **Simplified VAR**: The Simplified VAR contains the code which implements 3 different types of visual token redistribution model that attempt to provide performance improves over the baseline without the high computational cost from the VCD method.

### Datasets and Results
The provided `.zip` files contain the datasets, images, and raw experimental results associated with the standard multimodal benchmarks we used. You will need these to reproduce the project results:
- **`MME.zip`**: Data and resources related to the MME benchmark.
- **`MMVP.zip`**: Data and resources related to the MMVP benchmark.
- **`POPE.zip`**: Data and resources related to the POPE (Polling-based Object Probing Evaluation) benchmark.

## How to Use
1. Unzip the benchmark archive files (`MME.zip`, `MMVP.zip`, `POPE.zip`) into your working directory as required by the notebooks.
2. Run the **Baseline Model** notebook to evaluate the baseline hallucination metrics.
3. Run the **Reproduce VCD** notebook to evaluate the replication of VisAttnSink.
4. Run the **Simplified VAR** notebook to apply the efficient visual token redistribution models and observe the mitigation results.