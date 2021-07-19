# Machine Learning of all public <i>Pseudomonas aeruginosa</i> transcriptomes identifies independently modulated sets of genes associated with known transcriptional regulators

Data repository for applying independent component analysis decomposition on <i>P. aeruginosa</i> transcriptomic data as described in <i>biorxiv</i> 


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
  * <i>01_expression_QC_SOP</i> : Notebook to take raw reads and multiqc stats files. filtering thes samples, and produce log_tpm file
  * <i>02_expression_visualization</i> : Visualization of logTPM files by cluster map and PCA plots, and normalize the data (log_TPM_norm) 
  * <i>03_ica_dimensionality</i> : After running the ICA decomposition using nextflow, this notebook used to check the dimensionality to determine optimal M and A matrices
  * <i>04_ica_data_compile</i> : Compile various files and save it as single .json file
  * <i>05_ica_summary</i> : Summarize various iModulons in form of scatter plot on the basis of their functions
  * <i>06_simulation_CF</i> : Creates the heatmap, scatter plot, and barplots for the iModulons might have some role in Cystic Fibrosis 
  * <i>07_Carbon_AA_metabolism</i> : Notebook to various plots for Carbon and Amino Acid metabolism
  * <i>08_Clustermap</i> : Clustering all the iModulons based on similar functionality on the basis of Pearson correlation coefficient (PCC)
  * <i>09_Tradeoff</i> : Notebooks to create scatter plot between the RpoS and Translational iModulon 
  * <i>10_DIMAPlot</i> : Differential iModulon activity (DIMA) plot between the M9glucAA+Paraquat and M9glucAA      

* <b>Figures</b>
  * <i>Complete Figures</i>: 05 Figures which are used in main manuscript
  * <i>Supplementary Figures</i>: 06 Figures which are used as Supplemenatry figures

* <b>paeru_104_imodulon_ica.json</b> : .json files with all the information of 104 iModulons
* <b>README.md</b>



