# TNBC_MS023_ERV
## Introduction
This repository contain the ERV analysis of this paper:  
*PRMT inhibition induces a viral mimicry response in triple-negative breast cancer, 2022, Wu et. al..*  
The script for the analyses is written in R.
## Dependencies
This analysis requires:
+ DESeq2
+ ggplot2
+ ggrepel
+ pheatmap
## Reproducibility of the Analysis:
We use the [RepEnrich2](https://github.com/nerettilab/RepEnrich2) to estimate counts expression of repetitive element from RNA-seq FASTQ files, which the setting is recommended by the author of RepEnrich2.  
The "Data_and_Rscript" folder of this repo contains RepEnrich2 outcomes of each samples.  
 
+ Once the project is downloaded to the user computer, the user needs to navigate to the main directory of the project "TNBC_MS023_ERV". Running the "RepEnrich2_Downstream.R" will regenerate the ERV differential expression analysis plots used in the paper.

+ Note1: the user need to set the working directory inside the script file before running it.

+ Note2: We didn't use "Q3-MDAMB468-1uM_MS023-5d-replicate_1_S35_L002__fraction_counts" data because of its low mapping ratio during aligned it to reference genome. 
