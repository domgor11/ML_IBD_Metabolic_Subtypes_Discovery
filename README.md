# IBD_Metabolic_Subtypes_Discovery

This repository contains the code and data associated with the research project "Machine Learning-Driven Discovery of Metabolic Subtypes in IBD," authored by Dominika Gorgosz from the Department of Cancer and Genomic Sciences, School of Medical Sciences, College of Medicine and Health, University of Birmingham.

## Project Overview

This study addresses the significant challenge of heterogeneity in Inflammatory Bowel Disease (IBD) by identifying novel, biologically meaningful patient subtypes using untargeted serum metabolomics and unsupervised machine learning. I hypothesized that metabolomics, as a functional readout of host-microbiome pathophysiology, coupled with unsupervised machine learning, could enable the discovery of novel, biologically meaningful patient subtypes.

The primary objective was to move beyond conventional diagnostic boundaries (Crohn's disease (CD) and ulcerative colitis (UC)) to perform *de novo* discovery and characterization of robust metabolic subtypes within both CD and UC based on their distinct systemic metabolic signatures.

## Getting Started

To replicate the analyses in this project, please follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/domgor11/IBD_Metabolic_Subtypes_Discovery.git](https://github.com/domgor11/IBD_Metabolic_Subtypes_Discovery.git)
    cd IBD_Metabolic_Subtypes_Discovery
    ```

3.  **Download Raw Data:** 
    * The raw serum metabolomics data was obtained from the Integrative Human Microbiome Project (iHMP/IBDMDB) dataset.
    * Add `metadata.tsv` and `mtb.tsv` files to the `/raw_data` directory

4.  **Run the Notebooks:**
    The analysis workflow is organized into Jupyter notebooks. Please run them in sequential order:
    * `1_mtb_preprocessing.ipynb`
    * `2_daa_analysis.ipynb`
    * `3_boruta_feature_reduction.ipynb`
    * `4_permanova_analysis.ipynb`
    * `5_concordance_analysis.ipynb`
    * `6_signif_up_and_down_within_subtypes_daa.ipynb`
    * `7_lasso_analysis.ipynb`

## Contact

For any questions or inquiries, please contact Dominika Gorgosz at *dominika.gorgosz@alumni.bham.ac.uk*.


## Key Findings

**Two Robust Metabolic Subtypes:** Unsupervised clustering consistently identified two robust metabolic subtypes (a majority Cluster 0 and a minority Cluster 1) within both CD and UC populations.

**Opposing Metabolic Profiles:** The minority Cluster 1 was defined by a predominantly upregulated metabolic profile in CD but a predominantly downregulated profile in UC. Of the metabolites differentiating subtypes in both diseases, 99.7% exhibited this inverse relationship.

**Enhanced Clustering with Boruta Feature Set:** The Boruta-selected feature set (613 metabolites) yielded more stable clusters than the Differential Abundance Analysis (DAA) set (3,293 metabolites), dramatically improving clustering concordance in UC patients (Adjusted Rand Index (ARI) increased from 0.56 to 0.92).

**Minimal Biomarker Panels:** LASSO regression identified minimal, non-overlapping biomarker panels capable of perfectly discriminating these subtypes (16 features for CD, 7 for UC, with zero overlap).

**Conserved Metabolic Polarity:** These findings suggest a new framework for IBD pathophysiology where heterogeneity is driven by fundamental metabolic axes independent of traditional diagnostic boundaries, indicating a conserved metabolic polarity.

