## Fungal ITS Metabarcoding Analysis
Bioinformatics pipeline and statistical tests for processing Illumina paired-end ITS fungal sequencing data, using R and RStudio.

## Overview
This repository contains the scripts and data processing steps used in our study: "Leaf mycobiome across Fabaceae species: Non-nodulating plants exhibit higher fungal diversity."

For details regarding the software, parameters, and pipeline workflow, refer to the supplementary figure and attached files.

## Important information
1. **Data preprocessing and taxonomic assignment** 
   - Code is in the file Mycobiome_DADA2.Rmd
   - Tool: DADA2 (R package, version 1.34.0)
   - Inputs:
      - FASTQ sequencing files
      - UNITE database (sh_general_release_dynamic_25.07.2023.fasta)

2. **Statistical analysis and visualization**
   - Code is in the file Mycobiome_StatysticalAnalysis.Rmd
   - Tool: Vegan (R package, version 2.6.10)
   - Inputs:
      - Example dataset (provided in the repository)

