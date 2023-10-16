# Breast Cancer Gene Expression Analysis
Statistical analysis of gene expression in breast cancer cells to identify and model the impact of drug treatments

## Overview
This project aims to analyze gene expression data from breast cancer cells treated with different types and dosages of drugs. The primary focus is to identify genes whose expression is significantly altered by the treatments and to model these changes using Pearson correlation.

## Biological Background
<details>
  <summary>Overview of Drug Resistance Research</summary>

Biological Background Overview
Cancer therapies frequently fall short of achieving comprehensive and long-lasting responses due to the persistence of residual tumor clusters. These clusters display acquired resistance to drugs, posing a significant threat as they serve as the foundation for future relapse. Understanding the biological foundation of this inherent resistance is crucial, yet there is a noticeable absence of accurate in vitro models representing this state of cancer cells.

In recent observations, it's been noted that when breast and prostate cancer cells, derived directly from patients and cultured in 3D organoid formats, are treated with cytotoxic agents, a subset of these cells persists. These persistent cells not only display a unique phenotype but also showcase molecular characteristics that mimic the drug-resistant residual tumors found in clinical settings. This observation presents a promising avenue to understand the emergence and behavior of drug-refractory tumor cells.

</details>

## Dataset Overview
The dataset in focus offers RNAseq gene expression profiling data sourced from these persistent cancer cells. These cells were obtained after treating cancer organoids or PDX/xenograft tumors over time with:

Chemotherapeutic agents like docetaxel and vinblastine.
Targeted agents like afatinib.
By analyzing this data, we aim to pinpoint genes and pathways that are predominantly activated in these residual, drug-resistant tumors.

## Data Source
The gene expression data is sourced from the [GSE162285](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE162285).

## Tools and Libraries
- GitHub
- Bash/Linux
- Jupyter Lab
- Python
  - Pandas
  - Matplotlib
  - NumPy
  - Seaborn

## Project Structure
- `data/`: Contains the raw gene expression data.

## How to Run
1. Clone this repository.
2. Navigate to the project directory.
3. Run Jupyter Notebook for analysis.

## Methodologies and Analysis
**Data Loading and Exploration**: The gene expression data was initially loaded and explored to understand its structure and content.

### Data Cleaning and Preprocessing: 
- Gene identifiers were separated from their symbols for clarity. Sample names were simplified while ensuring differentiation between control and test samples.
- Gene expression values were normalized using the "Counts Per Million" (CPM) method.

### Data Visualization:

- Distribution of median expression values of all genes was plotted.
- A heatmap was generated to visualize expression levels of the top 50 genes with the highest median expression across samples.

### Statistical and Inferential Analysis:

- Median expression values of genes were computed for both control ("Veh" samples) and test groups ("Doc" and "Vinbl" samples).
- Differential expression analysis identified genes with significant expression differences between control and test groups.
- A correlation analysis was conducted for the top **ten** genes with the highest median expression to understand the relationships between them.

## Author
Aleksander Kossakowski

### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

### Literature references
GEO database: [NCBI GEO: archive for functional genomics data sets—update](https://academic.oup.com/nar/article/41/D1/D991/1067995?login=true)

Dataset: [An Embryonic Diapause-like Adaptation with Suppressed Myc Activity Enables Tumor Treatment Persistence](https://pubmed.ncbi.nlm.nih.gov/33417832/)
