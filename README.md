# Model-Agnostic Explanations by Consensus

## Authors

*   **Carlos Mencía**¹
*   **Ramon Béjar**²
*   **Raúl Mencía**¹
*   **Joao Marques-Silva**³

## Affiliations

¹ *Universidad de Oviedo, Spain*  
² *Universitat de Lleida, Spain*  
³ *ICREA & Universitat de Lleida, Spain*

---

## Abstract

This repository contains the datasets and experimental results presented in the paper: **"Model-Agnostic Explanations by Consensus"**, accepted at International Conference on Principles of Knowledge Representation and Reasoning, 2026.

## 🚀 Repository Structure

The repository is organized into three main directories:

### 1. `/datasets`
Contains the benchmark datasets used in our experiments:
*   `car`
*   `kr-vs-kp`
*   `corral` (de-duplicated)
*   `mux6` (de-duplicated)
*   `zoo` (de-duplicated)

Note: The original datasets belong to the UCI ML repository.

### 2. `/fixed-sample-analysis`
Contains the experimental results for the "Fixed-Sample Analysis" section of the paper. For each dataset, we provide the following metrics for every explained instance:
*   Number of **cbWAXps** found.
*   Size of the smallest **cbWAXp**.
*   Number of **necessary**, **not necessary**, and **relevant** features found.

### 3. `/evolution-under-sample-expansion`
Contains the data for the "Evolution Under Sample Expansion" section. For each dataset and expansion stage, there is a specific file named as follows:  
`[dataset_name]_[percentage_of_instances_to_explain]_[percentage_of_instances_in_sample].txt`

These files cover percentages from 5% to 100% (in 5% increments) and contain:
*   **Instance Lists:** The set of instances to be explained and the current sample instances.
*   **Metrics:** For each explained instance:
    *   Size of the smallest **cbWAXp**.
    *   Count of **necessary**, **not necessary**, and **relevant but not necessary** features identified.

Note about the results files: In the files, 'Instance i' corresponds to the i-th row of the corresponding dataset (starting at 1 and omitting the header).

## 📄 License

This project is licensed under the Creative Commons Zero v1.0 Universal License. See the `LICENSE` file for details.
