# Code for the work "Bioplastic Design using Multitask Deep Neural Networks"

This repository contains the code for the paper "Bioplastic Design using Multitask Deep Neural Networks" published at [Arxiv](https://arxiv.org/abs/xxxxxxx). The final predictors are not included in this repository, but can be accessed at [PolymerGenome](https://polymergenome.org).

## Install

```bash
git clone git@github.com:Ramprasad-Group/bioplastic_design.git
cd bioplastic_design
poetry install
```

## How to use

[search_space.ipynb](bioplastic_design/search_space.ipynb) -  Create a polymer search space (here bioplastic search space). Predictors are not included.

[screening.ipynb](bioplastic_design/screening.ipynb) - Use this notebook to screen for polymers with specific property values.
  
[candidates.txt](bioplastic_design/candidates.txt) - 70 bioplastic candidates for the 7 mainstream plastics (see paper for more information)