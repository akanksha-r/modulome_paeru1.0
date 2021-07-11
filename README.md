# Machine Learning of all public <i>Pseudomonas aeruginosa</i> transcriptomes identifies independently modulated sets of genes associated with known transcriptional regulators

Data repository for applying independent component analysis decomposition on <i>P. aeruginosa</i> transcriptomic data as described in <i>biorxiv</i> 

## Installation

## Repository Structure

* <b>Data</b>: Files created throughout the ICA decomposition and analysis process
  * External
     * Contains files extracted from external repositories e.g. KEGG and GO enrichments


  * iModulondb
    * Includes files to build iModulondb website

  * Interim
      * Contains data processed by pipeline and which is also required for further analysis

  * Processed Data
      * Includes the final data used for ICA analysis such as X, M, and A matrices as well as metadata and the Transcriptional Regulatory Netwrok (TRN) files

  * Raw Data
      * Contains the transcripts count and multiqc files of the data form SRA 
  
  * Sequence Files
      * Includes sequence files for <i> P. aeruginosa</i> PAO1


* <b>Notebooks</b>
  * 01_expression_QC_SOP : Notebook to take raw reads and multiqc stats files. filtering thes samples, and produce log_tpm file
  * 02_expression_visualization : Visualization of logTPM files by cluster map and PCA plots, and normalize the data (log_TPM_norm) 
  * 03_ica_dimensionality : After running the ICA decomposition using nextflow, this notebook used to check the dimensionality to determine optimal M and A matrices
  * 04_ica_data_compile : Compile various files and save it as single .json file
  * 05_ica_summary : Summarize various iModulons in form of scatter plot on the basis of their functions
  * 06_simulation_CF : Creates the heatmap, scatter plot, and barplots for the iModulons might have some role in Cystic Fibrosis 
  * 07_Carbon_AA_metabolism : Notebook to various plots for Carbon and Amino Acid metabolism
  * 08_Clustermap : Clustering all the iModulons based on similar functionality on the basis of Pearson correlation coefficient (PCC)
  * 09_Tradeoff : Notebooks to create scatter plot between the RpoS and Translational iModulon 
  * 10_DIMAPlot : Differential iModulon activity (DIMA) plot between the M9glucAA+Paraquat and M9glucAA      

* <b>Supplementary Files</b>
* <b>Figures</b>
* <b>paeru_104_imodulon_ica.json</b>
* <b>README.md</b>



