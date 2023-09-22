# Breast Cancer Gene Expression Analysis
Statistical analysis of gene expression in breast cancer cells to identify and model the impact of drug treatments

## Overview
This project aims to analyze gene expression data from breast cancer cells treated with different types and dosages of drugs. The primary focus is to identify genes whose expression is significantly altered by the treatments and to model these changes using statistical methods like Pearson correlation.

## Biological Background
<details>
  <summary>Overview of Drug Resistance Research</summary>

In the realm of cancer treatment, the persistent challenge of incomplete eradication and subsequent relapses arises due to the emergence of drug-resistant tumor cells. These cells, known as the "seed" for relapse, evade the effects of therapies and hinder successful long-term outcomes. Despite this significance, the underlying biological mechanisms driving _in situ_ resistance within tumors remain poorly understood. Moreover, the absence of accurate _in vitro_ models to simulate this drug-refractory state of cancer cells further complicates the study of this phenomenon.

The present investigation delves into comprehending the intricate dynamics of drug resistance in cancer treatment. The primary focus lies on breast and prostate cancer patient-derived cells and established cell lines, which are cultivated as 3D organoids in laboratory conditions. This novel approach aims to replicate the _in vivo_ conditions more accurately. By subjecting these organoids to cytotoxic treatments, such as conventional chemotherapy agents like _docetaxel_ and _vinblastine_, as well as targeted therapy with _afatinib_, the goal is to mimic the emergence of persistent tumor cell subpopulations observed during clinical treatments. The critical outcome of this endeavor is the generation of RNA sequencing (RNAseq) gene expression profiles from the drug-persistent cancer cells. These cells are cultivated from xenograft (PDX) tumors that were systematically exposed to chemotherapeutic or targeted agents. The RNAseq dataset obtained provides an invaluable resource for unraveling the genetic landscape of these drug-resistant tumor cells.

The utilization of this gene expression data offers a unique opportunity to identify specific genes and pathways that undergo upregulation in the context of drug-resistant residual tumors. Through meticulous analysis, researchers can uncover potential molecular drivers contributing to the development of drug-refractory states in cancer cells.

</details>

## Objectives
1. Identify pairs of genes whose expression levels are highly correlated.
2. Model how the expression levels of these genes change with different dosages of specific drugs.
3. Determine if the observed changes in gene expression are statistically significant.

## Data Source
The gene expression data is sourced from the [GSE162285](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE162285).

## Tools and Libraries
- GitHub
- Bash/Linux
- Jupyter Lab
- Python
  - Pandas
  - Matplotlib
  - SciPy
  - NumPy
  - Seaborn

## Project Structure
- `data/`: Contains the raw gene expression data.
- `notebooks/`: Jupyter notebooks for data exploration and analysis.

## How to Run
1. Clone this repository.
2. Navigate to the project directory.
3. Run Jupyter Notebook for analysis.

## Author
Aleksander Kossakowski

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

## Acknowledgments
The gene expression data is sourced from the [GEO database](https://www.ncbi.nlm.nih.gov/geo/).

## Literature references
GEO database: [NCBI GEO: archive for functional genomics data sets—update](https://academic.oup.com/nar/article/41/D1/D991/1067995?login=true)

Dataset: [An Embryonic Diapause-like Adaptation with Suppressed Myc Activity Enables Tumor Treatment Persistence](https://pubmed.ncbi.nlm.nih.gov/33417832/)
