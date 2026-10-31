# Code repository for "Molecularly-guided spatial proteomics captures single-cell identity of the healthy and diseased nervous system"

This repository contains analysis code associated with the manuscript:

**Molecularly-guided spatial proteomics captures single-cell identity of the healthy and diseased nervous system**  
*DOI: [10.1101/2025.02.10.637505](https://www.biorxiv.org/content/10.1101/2025.02.10.637505v2)*  
**Authors:**  
Sayan Dutta#, Marion Pang#, Gerard M. Coughlin, Sirisha Gudavalli,  
Michael L. Roukes, Tsui-Fen Chou, Viviana Gradinaru*

\# Equal contribution  
\* Corresponding author

**Code archive (Zenodo):** [10.5281/zenodo.21987350](https://doi.org/10.5281/zenodo.21987350)

The manuscript has been accepted for publication. This repository provides the Python notebooks used to generate the figures, together with the supplementary tables. Analyses rely on the authors’ open-source package [**scpviz**](https://github.com/gnaprs/scpviz).

## Contents

- `analysis_*.ipynb`  
  Python notebooks that perform the analyses and generate the figures.

- `environment.yml`  
  Conda environment used to run the notebooks.

- `supplementary tables/`  
  Supplementary tables and source data for the manuscript (see [Supplementary tables](#supplementary-tables) below).

## Data availability

### Supplementary tables

The supplementary tables are provided in [`supplementary tables/`](supplementary%20tables/):

- `Source data for graphs.xlsx`: source data for the graphs in the manuscript
- `Supp. Table 1_OmicsComparison.xlsx`: omics comparison
- `Supp. Table 2_dropviz data_SNpc_Cortex.xlsx`: Dropviz data for SNpc and cortex
- `Supp. Table 3_RNA-FISH-probes.xlsx`: RNA-FISH probes
- `Supp. Table 4_LaserCaptureMicrodissectionSettings.xlsx`: laser capture microdissection settings
- `Supp. Table 5_LCMSMSSettings.xlsx`: LC-MS/MS settings
- `Supp. Table 6_DE.xlsx`: differential expression results
- `Supp. Table 7_SampleCounts_Info.xlsx`: sample counts and information

### Raw mass spectrometry data

- **MassIVE:** [MSV000100704](https://massive.ucsd.edu/ProteoSAFe/dataset.jsp?task=dd7f039446bd4db79a506b35a8dbb312)
- **ProteomeXchange:** [PXD074008](https://proteomecentral.proteomexchange.org/ui?pxid=PXD074008)

Transcriptomic reference data were obtained from the Allen Brain Atlas and Dropviz, as described in the manuscript.

## Setup

Analyses were performed using **Python 3.11**.  
The complete software environment, including all dependencies and exact package versions, is provided in `environment.yml`.

To recreate the environment:

```bash
conda env create -f environment.yml
conda activate scpviz
```

This environment includes the authors' open-source analysis package [`scpviz`](https://github.com/gnaprs/scpviz) and all additional dependencies required to run the notebooks.
