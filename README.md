# ML IBD Metabolic Subtypes Discovery

This repository contains the code and data associated with the research project "Machine Learning-Driven Discovery of Metabolic Subtypes in IBD," authored by Dominika Gorgosz from the Department of Cancer and Genomic Sciences, School of Medical Sciences, College of Medicine and Health, University of Birmingham.

## Project Overview

This study addresses the significant challenge of heterogeneity in Inflammatory Bowel Disease (IBD) by identifying novel, biologically meaningful patient subtypes using untargeted serum metabolomics and unsupervised machine learning. I hypothesized that metabolomics, as a functional readout of host-microbiome pathophysiology, coupled with unsupervised machine learning, could enable the discovery of novel, biologically meaningful patient subtypes.

The primary objective was to move beyond conventional diagnostic boundaries (Crohn's disease (CD) and ulcerative colitis (UC)) to perform *de novo* discovery and characterization of robust metabolic subtypes within both CD and UC based on their distinct systemic metabolic signatures.

## Getting Started

To replicate the analyses in this project, please follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/domgor11/ML_IBD_Metabolic_Subtypes_Discovery.git
    cd ML_IBD_Metabolic_Subtypes_Discovery
    ```

3.  **Download Raw Data:** 
    * The raw serum metabolomics data was obtained from the Integrative Human Microbiome Project (iHMP/IBDMDB) dataset.
    * Add `metadata.tsv` and `mtb.tsv` files to the `raw_data/` directory

4.  **Run the Notebooks:**
    The analysis workflow is organized into Jupyter notebooks in the `notebooks/` directory. Please run them in sequential order:
    * `1_mtb_preprocessing.ipynb`
    * `2_daa_analysis.ipynb`
    * `3_boruta_feature_reduction.ipynb`
    * `4_permanova_analysis.ipynb`
    * `5_concordance_analysis.ipynb`
    * `6_signif_up_and_down_within_subtypes_daa.ipynb`
    * `7_lasso_analysis.ipynb`

## Contact

For any questions or inquiries, please contact Dominika Gorgosz at *dominika.gorgosz@alumni.bham.ac.uk*.

