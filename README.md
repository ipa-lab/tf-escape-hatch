# Artifact - Security Anti-Patterns in Terraform Modules: Identifying Risks in Provisioners and External Data Sources

This repository contains the artifact for our paper "Security Anti-Patterns in Terraform Modules: Identifying Risks in Provisioners and External Data Sources" submitted to the MSR 2026.


We present the first empirical study of escape hatches in Terraform modules. Analyzing all 17,019 modules from the public Terraform Registry, we find that 1,359 (7.96%) contain at least one escape hatches. Through qualitative analysis, we develop a taxonomy of ten recurring security smells that capture distinct implementation patterns and their associated risks.

## Structure

This repository is structured as follows:
- `raw-dataset/`: Contains our scripts to retrieve meta-data for all publicly available modules and the output meta-data.
- `analysis/`: Contains the data and scripts for reproducing to measure the prevalence of the identified security smells across the dataset. 
- `LICENSE`: The license file for the repository.

## Reproduction Instructions

### raw-dataset

For reproduction of the raw-dataset, run the following command in the `raw-dataset`:
```bash
python get-modules.py
```

### analysis:
For reproduction of the raw-dataset, run all scripts in the `analysis` folder
