# PARTAGE
Scripts for the analysis of PARTAGE data
Consists of four jupyter notebook files

PARTAGE_RT.ipynb: Used for calculating and plotting partage data. 
Requires RPKM data for G1 samples and other timepoints. Will output 
correlation graph and PARTAGE heatmap representing the replication 
timing.

rna_enrichment_corr.ipynb: Used for calculating clusters and 
enrichment analysis of expression data, along with self-correlation and 
correlation between pseudo-RT and expression.

CNV_Analysis_plot.ipynb: Used for plotting copy number variation along 
with called deletions and duplications called by CNVpytor. Outputs calls
text file for use with ProOvErlap

convert_calls_to_bed.ipynb: convert text file output to bed for
ProOvErlap
