# Quantitative Verification of In-Flight UAV Reconfiguration under Uncertainty

This repository contains the PRISM models and property specifications used in the paper  
"Quantitative Verification of In-Flight UAV Reconfiguration under Uncertainty", currently under review for submission to [EPEW 2026](https://epew-workshop.github.io).

The models capture reconfiguration decisions based on timing analysis and battery state information, enabling policy synthesis using probabilistic model checking.

## Repository Contents

- **UAV_model.prism**  
  The PRISM model encoding the Markov Decision Process (MDP) used to evaluate and synthesise runtime reconfiguration strategies for the UAV system under uncertainty.

- **properties.pctl**  
  The multi-objective PCTL property specifications used for policy synthesis, capturing constraints on timing, energy consumption, and assurance confidence.

- **MDP model generation/**  
  Contains the script `modelGen.py`, which generates the MDP model from a parameter file (`config.json`). The configuration file specifies system parameters such as execution-time bounds, energy consumption values, and probabilistic assumptions used in the case study.

## Requirements

- PRISM model checker: https://www.prismmodelchecker.org/