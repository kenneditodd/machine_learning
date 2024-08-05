# Rapid protein evolution by few-shot learning with a protein language model
## Goal
The goal of this directory is to reproduce the few-shot learning with a protein language model created in [Rapid protein evolution by few-shot learning with a protein language model](https://doi.org/10.1101/2024.07.17.604015)
## Background
- Jiang et al. 2024 utilized a previously published table containing single amino acid VEPs and DMS measurments used for benchmarking
  - [Using deep mutational scanning to benchmark variant effect predictors and identify disease mutations](https://doi.org/10.15252/msb.20199380)
- Used EMS2-12B protein language model
## 01_explore_and_scrub.ipynb
- User specifies the dataset (FASTA file), protein of interest (sheet/tab from Source.xlsx), fitness metric (column from Source.xlsx), and fitness cutoff value.
- Read **Source.xlsx**, scrub data, output labeled data, and generate 3 plots.
- Script contains 3 functions; 2 plotting functions and 1 data processing function.
- **Source.xlsx**
  - an excel file containing VEP measurements from 31 previously published DMS experiments for single amino acid subsitutions. This was used to benchmark 46 VEPs. Each tab is for a specific protein. Within each tab, rows are variants and columns are VEP or DMS metrics.
  - VEP = variant effect predictors, DMS = deep mutational scanning
  - DMS experiments combine saturation mutagenesis of a protein of interest with a high‐throughput functional testing and deep sequencing
## 02_extract_ESM.ipyng
- ESM = Evolutionary Scaling Model
- ESM2-15B is a protein language model with 15B parameters from [Meta](https://huggingface.co/facebook/esm2_t48_15B_UR50D). It is suitable for fine-tuning on a wide range of tasks that take protein sequences as input.
## Citation (preprint)
Rapid protein evolution by few-shot learning with a protein language model
Kaiyi Jiang, Zhaoqing Yan, Matteo Di Bernardo, Samantha R. Sgrizzi, Lukas Villiger, Alisan Kayabolen, Byungji Kim, Josephine K. Carscadden, Masahiro Hiraizumi, Hiroshi Nishimasu, Jonathan S. Gootenberg, Omar O. Abudayyeh
bioRxiv 2024.07.17.604015; doi: https://doi.org/10.1101/2024.07.17.604015
