# MDPI_Microorganism_Review_Emerging_and_Underdetected_CFs
Underlying data and scripts for figures

# Comparative analysis of ETEC colonization factor operons

This repository contains the R notebooks used to generate the comparative operon figures presented in:

> von Mentzer A. *Emerging and underdetected colonization factors of human enterotoxigenic Escherichia coli (ETEC): implications for surveillance and vaccine development.* (2026)

## Overview

The notebooks compare the genetic organization and protein conservation of human and animal-associated ETEC colonization factor (CF) operons.

The workflow:

- extracts CF operons from GenBank (`.gb`) and GFF/GFF3 annotation files;
- extracts and translates coding sequences (CDSs);
- calculates pairwise protein sequence identities between homologous genes;
- visualizes operon organization using **gggenes** with ribbons representing protein sequence similarity.

## Included analyses

- **κ-FUP adhesins:** CS13, CS23 and F4
- **γ2-FUP adhesins:** F6, CS12 and CS30

## Software

The notebooks were developed in **R** and make use of the following packages:

- tidyverse
- Biostrings
- pwalign
- gggenes
- grid

## Repository structure

```
.
├── kappa_CF_operon_comparison.Rmd
├── gamma_CF_operon_comparison.Rmd
├── data/
├── figures/
└── README.md
```

## Input data

The analyses use publicly available genome annotations obtained from GenBank/ENA. The accession numbers used in the manuscript are provided in the figure legends.

## Citation

If you use these notebooks, please cite the associated publication.

## Contact

Astrid von Mentzer  
Department of Infectious Diseases  
University of Gothenburg, Sweden

GitHub: https://github.com/vonMentzerLab
