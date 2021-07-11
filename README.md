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
  * 01_expression_QC_SOP
  * 02_expression_visualization
  * 03_ica_dimensionality
  * 04_ica_data_compile
  * 05_ica_summary
  * 06_simulation_CF
  * 07_Carbon_AA_metabolism
  * 08_Clustermap
  * 09_Tradeoff
  * 10_DIMAPlot      

* <b>Supplementary Files</b>
* <b>Figures</b>
* paeru_104_imodulon_ica.json
* README.md



