# Fungal ITS Metabarcoding Analysis
Bioinformatics pipeline and statistical tests for processing Illumina paired-end ITS fungal sequencing data.  

Repository for "Leaf mycobiome across Fabaceae species: Non-nodulating plants exhibit higher fungal diversity" manuscript.
# Structure
Data folder includes the UNITE database used for the taxonomic assignation  raw data example for statistical analysis and 
data/
├── 3biom-Mycobiome.xlsx #example raw data for statistical analysis
└── sh_general_release_dynamic_25.07.2023.fasta #database
scripts/
├── 01_dada2_pipeline.Rmd 
└── 02_statistical_analysis.Rmd 
