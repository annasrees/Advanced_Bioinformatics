# Advanced Bioinformatics Final Project
Anna Rees | Spring 2024 |
UVM Advanced Bioinformatics | prof. Princess Rodriguez

## Introduction and Background
As transcriptomics and next-gen sequencing expands in affordability and technology, the amount of gene expression data available explodes. Bioinformatic tools like HISAT2 and STAR were created with the intention of streamlining the bioinformatic pipeline and to more easily quantify gene expression. HISAT2 and STAR are two of the most prominent read alignment tools. It is important to understand the key differences in performance when comparing HISAT to STAR, as their alignment is a quintessential aspect of the process, and much of the results of these bioinformatic analyses hinge on the accuracy and precision of these aligners.

## Information on the data
In order to assess the performance of these two aligners, I have chosen a dataset which came from a study on the heterogeneity in a mouse model of metastatic breast cancer (accession number GSE165393). 
  GSE165393 is a dataset of organ-derived metastatic cell lines that were harvested from 10 female MMTV-PyMT mice. MMTV-PyMT female mice develop palpable mammary tumors which metastasize to the lung. Tumor-bearing organs from these mice were harvested for sample collection. These cell lines were isolated and sorted based on the expression of surface cancer markers, specifically CD44low/EpCAMhigh or CD44high/EpCAMhigh with previously sorted cell lines used as positive controls for comparison. To acquire the raw data for bulk RNA sequencing, total RNA was extracted using the QIAGEN RNeasy kit, with 2 distinct clonal isolate replicates per sample. A modified SMART-seq2 protocol was used to generate cDNA, and the Nextera XT DNA Sample Prep Kit was used to build Illumina libraries. Samples were then sequenced on a NextSeq500 with a minimum depth of 10 M reads.


This dataset is a compilation of counts files from 8 samples of mice tissue, which all have different treatments:

1. SRR13515350 - Bone Marrow, CD44 low (rep 1)
2. SRR13515351 - Bone Marrow, CD44 low (rep 2)
3. SRR13515352 - Bone Marrow, CD44 high (rep 1)
4. SRR13515353 - Bone Marrow, CD44 high (rep 2)
5. SRR13515354 - Lymph Node, CD44 low (rep 1)
6. SRR13515355 - Lymph Node, CD44 low (rep 2)
7. SRR13515356 - Lymph Node, CD44 High (rep 1)
8. SRR13515357 - Lymph Node, CD44 High (rep 2)

Each sample is either from Bone Marrow (BM), or Lymph Node (LN) tissue. The mouse either had high levels of CD44, a cell surface marker, or low levels of CD44.

## Skills gained
This semester-long project required extensive understanding of the entire bioinformatic pipeline, and knowledge of the technologies used to support bioinformatic research. All analysis was done through R. This is just a short list, since this course was the second of two semester-long comprehensive courses on bioinformatics, so there was much to learn!

- single-cell and bulk RNA-seq analysis
- familiarity w/ cancer biology
- Unix shell scripting
- Sequence alignment tools (STAR and HISAT)
- NGS workflow, data analysis, and pipeline management
- batch correction  
