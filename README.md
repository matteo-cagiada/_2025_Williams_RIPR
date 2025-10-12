# MD Analysis Notebook – Supplementary Information: t-SNE Evaluation

**Author:** Matteo Cagiada  
**Date:** October 2025  
**Version:** v1.0  
**Contact:** [matteo.cagiada@io.ku.dk](mailto:matteo.cagiada@io.ku.dk) / [matteo.cagiada@stats.ku.dk](mailto:matteo.cagiada@stats.ku.dk)

---

## 🧬 Overview

This Jupyter notebook accompanies the paper:

> **Synergistic relationships between non-neutralising antibodies targeting the essential *Plasmodium falciparum* RIPR protein drive inhibition of erythrocyte invasion**  
> Barnabas G. Williams, Jordan R. Barret, Josephin Bartholdson-Scott, Cassandra A. Rigby, Matteo Cagiada, Doris Quinkert, Kirsty McHugh, Anna Huhn, Sean Burnap, Sai Sundar Rajan Raghavan, Ana Rodrigues, Laura Bergamaschi, Beatrice Balzarotti, Simon Watson, Noah Miller, Lloyd King, Francesca Donnellan, Camilla Gladstone, Camille Gourjault, Jemima Paterson, Stefania Scalabrino, Katherine Skinner, Charlotte M. Deane, Stephen Reece, Jacqueline Kircher, Andrew Ward, and Simon J. Draper

This notebook contains the analyses, figures, and computational procedures of the molecular dynamics (MD) simulations of RIPR referenced in the main manuscript.  
All results can be reproduced following the instructions below.

---

## ⚙️ How to Run

### 1. Download the Simulation Data

Download all MD trajectories from the Zenodo repository:

🔗 **DOI:** [10.5281/zenodo.17315520](https://doi.org/10.5281/zenodo.17315520)

Place all downloaded files in the `src` folder located in the main directory of this repository.

---

### 2. Environment Setup

- **Python version:** 3.9+  
- **Recommended environment:** Conda  

#### Dependencies

The following Python packages are required:

numpy
MDAnalysis
seaborn
matplotlib
scipy
itertools
scikit-learn

### 3. Running the Notebook

Open the notebook in Jupyter and execute all cells in order:

```bash
jupyter notebook TSNE_analysis.ipynb
```

## 🧩 Simulation System Naming

The sections, variables, and figures in the notebook are labeled according to chain identifiers in the crystal structure.  
Below is a mapping between the simulation names used in the notebook and the corresponding system compositions:

| Notebook Label | System Description |
|----------------|--------------------|
| **ripr_all_domain** | RIPR + RP.035 + RP.047 + RP.057 + RP.063 + RP.073 + RP.093 |
| **ripr_LM_HI_JK_domain** | RIPR + RP.035 + RP.047 + RP.057 |
| **ripr_HI_JK_DE_domain** | RIPR + RP.052 + RP.047 + RP.057 |
| **ripr_BO_CD_EF_domain** | RIPR + RP.063 + RP.073 + RP.093 |
| **ripr_LM_JK_domain** | RIPR + RP.035 + RP.057 |
| **ripr_HI_JK_domain** | RIPR + RP.047 + RP.057 |
| **ripr_LM_BO_domain** | RIPR + RP.035 + RP.093 |
| **ripr_LM_domain** | RIPR + RP.035 |
| **ripr_HI_domain** | RIPR + RP.047 |
| **ripr_JK_domain** | RIPR + RP.057 |
| **ripr_BO_domain** | RIPR + RP.093 |
| **ripr_DE_domain** | RIPR + RP.052 |
| **ripr_only** | RIPR alone |

---

## 📫 Contact and Support

For questions, feedback, or issues reproducing results:

📧 **Email:** [matteo.cagiada@io.ku.dk](mailto:matteo.cagiada@io.ku.dk) / [matteo.cagiada@stats.ku.dk](mailto:matteo.cagiada@stats.ku.dk)  
🏛️ **Affiliation:** Department of Biology, University of Copenhagen  

---

## 📝 Citation

If you use this notebook or associated data, please cite:

> Williams *et al.*, *Synergistic relationships between non-neutralising antibodies targeting the essential Plasmodium falciparum RIPR protein drive inhibition of erythrocyte invasion*, [Journal Name], [Year], [DOI].


```markdown
## ⚖️ License

This repository and associated notebooks are distributed under the **MIT License**.
