
# RNA Seq Analysis

A computational workflow for the detection of DE genes and pathways from RNA-Seq data by providing a complete analysis of an RNA-Seq experiment profiling Drosophila cells after the depletion of a regulatory Pasilla gene.

In the study of [Brooks et al. 2011](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3032923/), the authors identified genes and pathways regulated by the Pasilla gene (the Drosophila homologue of the mammalian splicing regulators Nova-1 and Nova-2 proteins) using RNA-Seq data. They depleted the Pasilla (PS) gene in Drosophila melanogaster by **RNA interference (RNAi)**. Total RNA was then isolated and used to prepare both single-end and paired-end RNA-Seq libraries for treated (PS depleted) and untreated samples. These libraries were sequenced to obtain RNA-Seq reads for each sample. The RNA-Seq data for the treated and the untreated samples has been compared to **identify the effects of Pasilla gene depletion on gene expression.**

**4 untreated samples**: GSM461176, GSM461177, GSM461178, GSM461182\
**3 treated samples** (Pasilla gene depleted by RNAi) : GSM461179, GSM461180, GSM461181

Details about each step followed can be found in the [documentation](Documentation.pdf).\
All the tools were used on the Galaxy Europe server. 

## Steps

- Quality Control using FastQC, CutAdapt and MultiQC
- Mapping using STAR
- Inspection of results using IGV
- Counting reads using featureCounts
- DGE analysis using DESeq2
- Gene Ontology analysis using goseq
- KEGG pathway analysis

## Workspace
[Galaxy workspace (history)](https://usegalaxy.eu/u/nomad/h/rnaprofilingdrosophila).