# BIOT 6900 coursework
Name: Yuehua Deng
## Module 6
### Project Description
In this assignment, I calculated a polygenic risk score (PRS) using real genotype data and evaluated its portability across five ancestry groups: EUR, AFR, EAS, SAS, and AMR.
I performed allele harmonization, calculated PRS distributions, evaluated discrimination using AUC and calibration, and compared age-only with age-plus-PRS models.
### Data Sources
Course-provided data files: 
- genotypes.csv, variants.csv, score.csv, and meta.csv.
The phenotype labels were simulated rather than obtained from real patient diagnoses.
### Issues Encountered
None
## Module 5
### Research gene:CYP2C19
This repository contains my completed Module 5 variant interpretation assignment.
The submitted files include the completed Jupyter Notebook, the classified variant CSV file, and the report PDF.
## Module 4 
Targets: PGR and BCHE
This repository contains my Module 4 assignment for structure prediction and structure-based druggability analysis.
Files:
BIOT6900_Module4_Assignment.ipynb
structure_assessment_ov.csv — summary of the structural assessment
Module 4 Assignment.pdf
## Module 3 
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
### Data Sources
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
## Module 1 
Parts A–C completed.
Part D will be covered in the next class.
