# malaria-drone-cea
Cost-Effectiveness of Drone-Based Commodity Delivery Compared to Land-based Delivery in Remote Madagascar 

# Cost-Effectiveness of Drone-Delivered Malaria Interventions in Madagascar

## Overview
This repository contains the Python-based model and analytical code used to evaluate the cost-effectiveness of drone delivery for malaria testing and treatment commodities. 

The analysis is based on a Markov cohort model evaluating clinical and economic outcomes for children under 5 years of age in a rural Malagasy population. The model compares standard trial-informed supply chains against various drone scale-up scenarios.

## Repository Structure
The analysis is modularized into three primary execution files, intended to be run in the following sequence:

* `1_Copy_of_Inputs_Drone_CEA.ipynb`
    * Generates the tables of the key epidemiological, cost, and health-system parameters used in the model.
* `2_Copy_of_Deterministic_Drone_CEA.ipynb`
    * Contains the core deterministic Markov cohort model.
    * Calculates base-case transition probabilities, tracks the service pathway (testing and prompt treatment), and calculates deterministic Incremental Cost-Effectiveness Ratios (ICERs) and DALYs averted over 1-year and 10-year time horizons.
    * Includes the epidemiological face-validation exercise comparing model incidence outputs against empirical bounds from routine facility data.
* `3_Copy_of_PSA_Drone_CEA.ipynb`
    * Executes the Probabilistic Sensitivity Analysis (PSA).
    * Propagates parameter uncertainty through the Markov model via Monte Carlo simulation to generate cost-effectiveness acceptability curves (CEACs) and CEA plane.

## Usage and Reproducibility
The code is written in Python 3 and was developed using Google Colab. The easiest way to reproduce these results is to open the `.ipynb` files directly in Google Colab or Jupyter Notebook. 

**Dependencies:**
* `numpy`
* `pandas`
* `matplotlib` / `seaborn` (for figures)

## Citation
If you use this code or model structure in your research, please cite the accompanying manuscript and this repository:

**Cost-Effectiveness of Drone-Based Commodity Delivery Compared to Land-Based Delivery in Remote Madagascar**

Authors: Tara Templin, Takhona G. Hlatshwako, Eunice Kioko, Erica Felker-Kantor, Kanto Jude Ramanamahefa, Daniel Crapper, Sean Sylvia, Katherine Tumlinson

## License
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details. You are free to use, modify, and distribute this code for academic or commercial purposes, provided attribution is given to the original authors.
