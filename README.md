# BIOT 6900 coursework

Name: Yuehua Deng

## Module 3 

Name: Yuehua Deng

Disease: OV

Files included:
- BIOT6900_Module3_Assignment.ipynb
- targets_ov_w3.csv
- Module 3 Assignment — Computational Lab 3.pdf

Notes:
All top 15 targets were successfully mapped to the reviewed human proteome. The notebook ran successfully and the Module 3 analysis was completed.

## Module 2 

### Disease
Ovarian cancer

## Data Sources

### 1. Transcriptomics
- Dataset: E-GEOD-40595
- Data type: Differential gene expression
- Comparison used: ovarian cancer vs normal in epithelial cells
- Platform: Expression Atlas
- Columns used:
  - gene
  - log2 fold change
  - p-value
- Access: Open
- Source:
  https://www.ebi.ac.uk/gxa/experiments/E-GEOD-40595

### 2. Proteomics
- Dataset: CPTAC pan-cancer ovarian cancer cohort
- Data type: Gene-level proteomics
- Groups used:
  - Proteomics (Tumor)
  - Proteomics (Normal)
- Effect calculation:
  mean tumor protein abundance - mean normal protein abundance
- Statistical test:
  Welch's t-test
- Access: Open
- Source:
  https://www.linkedomics.org/data_download/CPTAC-pancan-OV/

### 3. Genomics
- Dataset: CPTAC pan-cancer ovarian cancer cohort
- Data type: Gene-level somatic mutation
- Genomic evidence:
  mutation frequency across tumor samples
- Access: Open
- Source:
  https://www.linkedomics.org/data_download/CPTAC-pancan-OV/

The CPTAC ovarian RNA tumor-only expression matrix was explored during data selection but was not used in the final transcriptomic scoring because it did not provide a tumor-vs-normal effect and p-value.

## Module 1 Assignment
Parts A–C completed.
Part D will be covered in the next class.
