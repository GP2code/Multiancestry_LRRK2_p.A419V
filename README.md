# The LRRK2 p.A419V risk variant influences age of onset for Parkinson's disease in East Asian populations

`GP2 ❤️ Open Science 😍`

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17701937.svg)](https://doi.org/10.5281/zenodo.17701937)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


## Summary
This is the online repository for the manuscript titled "The LRRK2 p.A419V risk variant influences age of onset for Parkinson's disease in East Asian populations". This study aims to resolve inconsistencies in previous reports by providing robust evidence that that the LRRK2 p.A419V is a significant risk player for PD in the EAS population while looking into data from multiple ancestries. The study also explores the variant's association with age at onset.

## Data Statement
- All GP2 data are hosted in collaboration with the Accelerating Medicines Partnership in Parkinson's Disease and are available via application on the website. The GP2 PD case and control data are available via the GP2 website (https://gp2.org; release 9: [https://doi.org/10.5281/zenodo.10472143](https://zenodo.org/records/14510099)). Genotyping imputation, quality control, ancestry prediction, and processing were performed using GenoTools (v1.0.0), publicly available on GitHub
- UKB statement?
- The All of Us genomic data are available under restricted access for human subject data. Access can be obtained by following the instructions under the All of Us workbench
- For EAS-WES data, Individual-level genotype data will be made available upon reasonable request and after approval by the relevant institutional review board. Please refer to Data availability section in Chew, E.G., Liu, Z., Li, Z. et al. Nat Aging. 2025 (https://doi.org/10.1038/s43587-024-00760-7) for more information.

# Repository Orientation
```
THIS_REPO
└── README.md
└── analysis
    └── AMP-PD
    |   └── 01_A419V_AMP-PD.ipynb    
    ├── GP2
    |   ├── 00_A419V_data_preparation.ipynb
    |   ├── 01_A419V_variant_analysis_release9.ipynb
    |   ├── 02_A419V_haplotype_release9.ipynb
    |   └── 03_A419V_AAO_analysis_release9.ipynb
    └── AllOfUs


```

## Notebooks Description
- Languages: Python, bash, and R

|Directory| Notebook                                 |Description                                                 |
|:--------|:-----------------------------------------|:-----------------------------------------------------------|
|GP2/     | 00_A419V_data_preparation.ipynb          |  Downloading and structuring data                          | 
|         | 01_A419V_variant_analysis_release9.ipynb |  Analyzes GP2 genotyped data across ancestries             | 
|         | 02_A419V_haplotype_release9.ipynb        | Analyzes haplotype around A419V in GP2 genotyped data      |
|         | 03_A419V_AAO_analysis_release9.ipynb     | Analyzes Age of Onset for PD A419V carrier and non-carrier |
|AMP-PD/  | 01_A419V_AMP-PD.ipynb                    | Analyzes AMP-PD whole-genome sequencing data               |
|AllOfUs/ | 01_LRRK2_A419V_AllofUs.ipynb             | Analyzes All-of-us whole-genome sequencing data               |

# Software
|       **Software**                | **Version(s)** |           **Resource URL**                                           |   **RRID**     |                                                               **Notes**                                               |
|:---------------------------------:|:--------------:|:--------------------------------------------------------------------:|:--------------:|:---------------------------------------------------------------------------------------------------------------------:|
| Python Programming Language       |3.10            |http://www.python.org/                                                | RRID:SCR_008394| pandas; numpy; seaborn; matplotlib; statsmodel; rpy2; used for general data wrangling/plotting/analyses                     |
|R Project for Statistical Computing|4.4.2           |http://www.r-project.org/                                             | RRID:SCR_001905| tidyverse; dplyr; tidyr; ggplot2; car; cowplot; grid; RColorBrewer; forestmodel; survival; used for general data wrangling/plotting/analyses|
|PLINK                              |1.9 and 2.0     |http://www.nitrc.org/projects/plink                                   | RRID:SCR_001757| used for genetic analyses                                                                                             |

