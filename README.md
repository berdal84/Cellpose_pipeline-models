# Cellpose_pipeline-models
![Cellpose Pipeline - Automated cell segmentation for retinal organoids](./resources/pipeline_overview.png)
---
Supporting software for the research paper: *"Retinoic acid drives cell fate specification and maturation in human retinal organoids"*
---
## Research paper
- *Authors*: Benjamin Y. Lim, Carissa Chen, Anna Fredericks, Elham Nilli, Santiago Mesa Mora, Megan Weathestone, To Ha Loi, Peter Newman, Nader Aryamanesh, Hala Zreiqat, Patrick Tam, Pengyi Yang, Anai Gonzalez-Cordero
- *Publication*: [Publication details forthcoming]
- *DOI*: [Forthcoming]
- *Repo*: https://github.com/blim934/Cellpose_pipeline-models
### Key findings
- Retinoic acid (RA) signaling functions as a primary morphogen regulating multiple aspects of human retinal organoid development
- High RA maintains progenitor proliferation and promotes rod specification, while low RA favors differentiation into cones, RGCs, and bipolar cells
- Low RA accelerates photoreceptor maturation, promoting outer segment formation and phototransduction protein expression
- RA levels establish regional retinal identity, with low RA promoting central/macular transcriptomic signatures and high RA driving peripheral fate
## About this software
This repository contains the image analysis pipeline developed to automate cell segmentation and quantification for the paper's retinal organoid experiments. The custom Cellpose models were trained specifically for retinal cell types and used for analyzing thousands of images across multiple experimental conditions.
### Installation
shell
'''
conda create -n cellpose_pipeline python==3.9 pip
conda activate cellpose_pipeline
git clone https://github.com/blim934/Cellpose_pipeline-models.git
cd Cellpose_pipeline-models  
pip install -r requirements.txt
'''
### Key features
- *GUI interface* to search and process folders of .czi, .lif, and .tif files
- *Maximum Intensity Projections (MIPs)* generation in various formats
- *Automated cell segmentation* using custom-trained Cellpose models
- *Cell-type specific morphometric analysis* with quantitative measurements
- *Multi-format support* (.czi, .lif, .tif) with batch processing
- *GPU acceleration* when available via CUDA or MPS
### How we used this software in our research
This pipeline was essential for analyzing the effects of retinoic acid modulation on retinal development:
- Quantified cell type proportions across different RA treatments
- Analyzed spatial distribution of different cell populations
- Generated datasets for statistical comparisons between experimental conditions
For detailed methods and results, please refer to the full paper.
### Citation
If you use this software or our findings in your research, please cite:
Lim, B.Y., Chen, C., Fredericks, A., et al. (2025). Retinoic acid drives cell fate specification and maturation in human retinal organoids. [Journal information forthcoming].
### License
CC0-1.0 license
