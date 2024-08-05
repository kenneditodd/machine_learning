# Rapid protein evolution by few-shot learning with a protein language model
## Goal
The goal of this directory is to reproduce the few-shot learning with a protein language model created in [Rapid protein evolution by few-shot learning with a protein language model](https://doi.org/10.1101/2024.07.17.604015)
## Background
- Jiang et al. 2024 utilized a previously published table containing single amino acid VEPs and DMS measurments used for benchmarking
  - [Using deep mutational scanning to benchmark variant effect predictors and identify disease mutations](https://doi.org/10.15252/msb.20199380)
  - VEP = variant effect predictors, DMS = deep mutational scanning
  - There are issues with VEPs being heavily biased and DMS in an alternative
  - DMS experiments combine saturation mutagenesis of a protein of interest with a high‐throughput functional testing and deep sequencing
  - **Source.xlsx** is an excel file containing VEP and DMS measurements from 31 previously published experiments for single amino acid subsitutions to benchmark 46 VEPS. Each tab is for a specific protein. Within each tab, rows are variants and columns are VEP/DMS predictions.
## Citation (preprint)
Rapid protein evolution by few-shot learning with a protein language model
Kaiyi Jiang, Zhaoqing Yan, Matteo Di Bernardo, Samantha R. Sgrizzi, Lukas Villiger, Alisan Kayabolen, Byungji Kim, Josephine K. Carscadden, Masahiro Hiraizumi, Hiroshi Nishimasu, Jonathan S. Gootenberg, Omar O. Abudayyeh
bioRxiv 2024.07.17.604015; doi: https://doi.org/10.1101/2024.07.17.604015
