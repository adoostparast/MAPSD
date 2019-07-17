# Markov Affinity-based Proteogenomic signal Diffusion (MAPSD)
MAPSD is a multi-omic signal diffusion algorithm designed to identify the disease susceptibility scores in unknown genes (or proteins) in complex and polygenic diseases such as schizophrenia.
# MAPSD Input arguments
MAPSD receives four input arguments including: Interactome (Network), Tissue-wise protein abundances, subcellular localization information for proteins, biological evidences for each gene.
* **Network**
Network is a text file with no headers and two columns where each row represents the source and target proteins. MAPSD currently only supports Ensembl gene IDs as input.
