# Code for paper: Bioplastic Design using Multitask Deep Neural Networks

# IMPORTANT NOTE: The code and data shared here is available for academic non-commercial use only

This repository contains the code for the paper "Bioplastic Design using Multitask Deep Neural Networks" published at [Arxiv](https://arxiv.org/abs/2203.12033). It contains two notebooks that show the creation of the bioplastic search space and screening of bioreplacements for commodity plastics. The predictors are not included in this repository but are made available as a part of the [PolymerGenome](https://polymergenome.org) project.

Abstract:

Non-degradable plastic waste stays for decades on land and in water, jeopardizing our environment; yet our modern lifestyle and current technologies are impossible to sustain without plastics. Bio-synthesized and biodegradable alternatives such as the polymer family of polyhydroxyalkanoates (PHAs) have the potential to replace large portions of the world's plastic supply with cradle-to-cradle materials, but their chemical complexity and diversity limit traditional resource-intensive experimentation. In this work, we develop multitask deep neural network property predictors using available experimental data for a diverse set of nearly 23000 homo- and copolymer chemistries. Using the predictors, we identify 14 PHA-based bioplastics from a search space of almost 1.4 million candidates which could serve as potential replacements for seven petroleum-based commodity plastics that account for 75% of the world's yearly plastic production. We discuss possible synthesis routes for these identified promising materials. 


## Install

```bash
git clone git@github.com:Ramprasad-Group/bioplastic_design.git
cd bioplastic_design
poetry install
```

## How to use

[search_space.ipynb](bioplastic_design/search_space.ipynb) - Create a polymer search space (here bioplastic search space). Predictors are not included.

[screening.ipynb](bioplastic_design/screening.ipynb) - Use this notebook to screen for polymers with specific property values.
  
[candidates.txt](bioplastic_design/candidates.txt) - 70 bioplastic candidates for the 7 mainstream plastics (see paper for more information)

[predictions_01_11_2022.parquet](bioplastic_design/predictions_01_11_2022.parquet) - The nearly 1.4 million bioplastic candidates, including property predictions. Load with `pd.read_parquet('predictions_01_11_2022.parquet')`
