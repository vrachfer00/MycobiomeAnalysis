## Fungal ITS Metabarcoding Analysis
Bioinformatics pipeline and statistical tests for processing Illumina paired-end ITS fungal sequencing data, using R software v4.3.2. 

## Overview
This repository contains the scripts and data processing steps used in our study titled "Leaf mycobiome across Fabaceae species: Non-nodulating plants exhibit higher fungal diversity". In the attached code files, we detail the software and parameters used.

## Pipeline Steps
1. **Data preprocessing and taxonomic assignment** 
   - Code is in the file Mycobiome_DADA2.Rmd 
   - Tool: DADA2 (R package, version 1.34.0)
   - Database: UNITE sh_general_release_dynamic_25.07.2023.fasta
   - Quality filtering using DADA2 (truncLen=250, maxEE=2, truncQ=2)
   - Removal of chimeric sequences (method="consensus")
     
2. **Statistical Analysis**
   - Code is in the file Mycobiome_StatysticalAnalysis.Rmd. Example data is also attached in the repository.
   - Tool: Vegan (R package, version 2.6.10)
   - Alpha diversity: ASV ruchness, Shannon, Pielou. Differences between nodulation statuses and plant subfamilies were tested using the Wilcoxon rank-sum test  
   - Beta diversity: Distance matrix calculated using Bray-Curtis dissimilarity + PERMANOVA (1000 permutations) 
