# Markov Affinity-based Proteogenomic signal Diffusion (MAPSD)
MAPSD is a multi-omic signal diffusion algorithm designed to identify the disease susceptibility scores in unknown genes (or proteins) in complex and polygenic diseases such as schizophrenia.
# MAPSD Input arguments
MAPSD receives four input arguments including: Interactome (Network), Tissue-wise protein abundances, subcellular localization information for proteins, and biological evidences for each gene.
* **Network:**
Network is a text file with no headers and two columns where each row represents the source and target proteins. MAPSD currently only supports Ensembl gene IDs as input.
* **Localization:** Localization is a CSV file curated from Human Protein Atlas which denotes where in each cell a protein is expressed. We encourage users to leave this file intact.
* **Protein:** Protein is a CSV file which contains the tissue and cell-specific abundances of proteins in the human body. Users are encouraged to use this file directly without further modification.
* **Evidence:** Evidence is a text file with no header and two columns. The first column represents the protein Ensemble ID (e.g., ENSG00000174640) and the second column denotes its corresponding signal (which is a Natural number). For instance if a gene is differentially expressed and also differentially methylated, then its signal value will be 2.
# How to run MAPSD 
MAPSD is written in R 3.5.1 but should be runnable on newer versions, too. Users need to download the MAPSD.rar file, unzip it, and run the following script in Linux terminal: Rscrip MAPSD.R. MAPSD can also be directly executed in R. Users can modify the Network and Evidence files based on their context under study but they are highly encouraged not to modify the Localization and Protein files.
MAPSD will generate a CSV file named "Final.csv" which includes the propogated disease signals for all of the proteins in the network and >100 combinations of tissues and cell-types.
# Support
In case of further assistance, users can contact me at doostparaa@email.chop.edu.
