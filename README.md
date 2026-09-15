# Overview

This project aims to determine whether 3D intestinal chicken organoids can measure breed-specific differences in chickens. Specifically, it analyses gene expression data from 90 genes associated with bacterial invasion (Avian Pathogenic Escherichia coli) as well as nutrition-related genes.

# Fluidigm_data_analysis

This Python script is designed to automatically analyze normalized qPCR data obtained from Fluidigm runs. It performs multiple comparisons across different groups, which must be defined in the metadata at the end of the CSV file before uploading.

The initial data is normalized against corresponding plates or reference genes using the GenEx software.

# Objectives

- Analyse experimental gene expression data
- Compare responses between experimental groups
- Visualise differences between conditions
- Identify genes associated with the host response to infection

# Methods

The analysis was performed using Python, including:

- pandas
- NumPy
- matplotlib
- seaborn
- SciPy
- scikit-learn 


# Results
[to be published in manuscript]
- Code will join and label data as well as check for data errors
- It will categorise genes into groups, providing a consistent colour scheme. The example genes used in this code are: barrier_function; gut_hormone; nutrient_receptors; immune_response; nutrient_transporters; metabolism; oxidation and ref_genes.
- Provides violin plots across gene categories for QC
- Compares uninfected treatment groups and produces Venn diagrams of significantly differentially expressed genes (DEGs) and bar plots of unique DEGs.
- Provides volcano plots of treated vs untreated groups in different conditions
- Provides Venn diagrams of DEGs overlapping between treated groups within different conditions. For shared genes, it provides a scatterplot, and for unique DEGs it provides bar plots. 

Author
Taylor R. Hanford, PhD
