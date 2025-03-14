# Multi-Omics Analysis of Alzheimer’s Disease Risk Factors in Microglia

## Project Overview
Microglia, the brain’s resident immune cells, play a crucial role in neurodegenerative diseases like Alzheimer’s, glaucoma, and multiple sclerosis. However, the mechanisms linking non-coding genetic risk variants to dysregulated gene expression remain poorly understood.

This project integrates multi-omics data—including differential gene expression profiles, microglia-specific cis-regulatory elements (CREs) from ATAC-seq, and transcription factor (TF) networks inferred from single-cell RNA-seq (scRNA-seq) and protein interaction databases—to uncover key regulatory mechanisms driving Alzheimer’s disease (AD) pathology.

## Objectives
- Conduct differential expression analysis on RNA-seq data to assess the impact of AD risk factors on microglial gene regulation.
- Integrate ATAC-seq and bulk RNA-seq data to identify key regulatory elements and transcription factors (TFs) associated with expression changes.
- Investigate additional risk factors beyond IFN-beta and explore regulatory changes using scRNA-seq data.
- Map disease-associated genes to their regulatory elements using eQTL data and TF-mediated interactions.

## Repo Structure 

**DEA/** – Contains R scripts for differential expression analysis (DEA) and multi-omics integration
- Differential_Expression_Analysis.Rmd – R Markdown file for RNA-seq differential expression and ATAC-seq integration
- functions.R – Custom functions used for analysis

**Gene_Mapping/** – ATAC-seq/epigenetic analysis and mapping
- Nextflow pipeline: Includes common Nextflow directories and configuration files
  - main.nf – Main pipeline script
  - config/ – Configuration files for pipeline execution
  - modules/ – Nextflow modules for ATAC-seq and mapping steps

## Data Availability
**Note**: Due to ongoing research and pending publication, data and result files are not included in this repository at this point.

## Future Work
- Expand the analysis to additional Alzheimer’s disease risk factors.
- Integrate single-cell RNA-seq data to infer TF networks and gene regulatory interactions.
- Link CREs to their target genes via eQTLs and other epigenetic mechanisms.

## Tools and Dependencies
- RNA-seq & ATAC-seq analysis: R, DESeq2, ATACseqQC, bedtools
- Pipeline automation: Nextflow, Docker
- Data visualization: ggplot2 - PCA, Volcano Plot, GSEE etc

