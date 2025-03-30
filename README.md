## Fungal ITS Metabarcoding Analysis
Bioinformatics pipeline and statistical tests for processing Illumina paired-end ITS fungal sequencing data, using R software v4.3.2. 

## Overview
This repository contains the scripts and data processing steps used in our study titled "Leaf mycobiome across Fabaceae species: Non-nodulating plants exhibit higher fungal diversity". Below, we detail the software and parameters used.

## Pipeline Steps
1. **Data Preprocessing (R package, version 1.34.0) ** 
   - Quality filtering using DADA2 (truncLen=250, maxEE=2, truncQ=2)
   - Removal of chimeric sequences (method="consensus")
2. **Taxonomic Assignment**  
   - BLASTn against NCBI database  
3. **Statistical Analysis**  
   - Alpha diversity: Shannon, Simpson (vegan package)  
   - Beta diversity: Bray-Curtis distance + PERMANOVA
