# MDPI_Microorganisms_Review_Emerging_and_Underdetected_CFs

This repository contains the underlying data and R notebooks used to generate figures presented in:

> von Mentzer A. *Emerging and underdetected colonization factors of human enterotoxigenic Escherichia coli (ETEC): implications for surveillance and vaccine development.* (2026)

## Overview

The notebooks compare the genetic organization and protein conservation of human- and animal-associated enterotoxigenic *Escherichia coli* (ETEC) colonization factor (CF) operons.

The workflow:

- extracts CF operons from GenBank (`.gb`) files;
- extracts and translates coding sequences (CDSs);
- calculates pairwise amino acid sequence identity between homologous proteins;
- visualizes operon organization using **gggenes**, with ribbons representing pairwise protein sequence identity.

## Included analyses

### Figure 1. Prevalence of CFs over time in Bangladesh
The repository contains the R notebook used to generate a heatmap summarizing the reported prevalence of human ETEC colonization factors across published studies.

### Figure 2. Comparative organization of κ-FUP adhesin operons

The repository contains the R notebook used to generate the comparison of the κ-FUP adhesin operons:

- **CS13** (OU964063)
- **CS23** (JQ434477)
- **F4** (CP002730)

The notebook extracts the operons, translates all coding sequences, calculates pairwise amino acid sequence identity between homologous proteins, and generates the publication-quality operon comparison figure.

## Software

The notebooks were developed in **R** using:

- tidyverse
- ggplot2
- dplyr
- Biostrings
- pwalign
- gggenes
- grid

## Input data

The analyses use publicly available genome annotation files obtained from GenBank and ENA. Accession numbers for all genomes analysed are provided in the corresponding figure legends in the manuscript.

## Citation

If you use these notebooks or data, please cite the associated publication.

## Contact

**Astrid von Mentzer**  
Department of Infectious Diseases  
University of Gothenburg, Sweden  

Email: astrid.von.mentzer@gu.se

GitHub: https://github.com/vonMentzerLab
