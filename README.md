# GeneTarget : A tool to identify genotype-treatment response
<img src="https://user-images.githubusercontent.com/41301333/195215088-8404f200-8297-4322-a30f-c84f526aa620.png" width="300" height="300">


##  Abstract
For a number of neurological diseases, such as Alzheimer's disease, Parkinson's disease and many others, certain genes are known to be involved in the disease mechanism.
A common question is whether a structural variant in any such gene may be related to drug response in clinical trials, and how this relationship can contribute to the lifecycle of drug development.
To this end, we introduce \<GeneTarget\>, a tool that identifies changes in survival relative to structural variants within target genes. 


##  Introduction

The challenges in developing novel therapeutics for neurodegenerative diseases (ND) result from the paucity of novel, valid targets. This in turn results from etiological heterogeneity, the complex and often polygenic nature of genetic risk. Despite the increase in funding for drug discovery, only 10% of new drug candidates in early stage clinical trials are eventually approved. Recent study has found that drug targets with genetic support were twice as likely to be approved. The discovery of rare and common genetic variants associated with risk for neurological and neuropsychiatric illness provides the opportunity to restart hypothesis-led clinical trials data analysis. High-risk mutations in single genes that identify specific targets for manipulation such as PCSK9, where identification of individuals with knockout mutations and benign lower LDL cholesterol has led to promising results in clinical trials and the development of evolocumab (Amgen) and alirocumab (Regeneron). In clinical practice and biomedical research, next-generation sequencing (NGS) and subsequent identification of genomic variants including single nucleotide variations, small insertions or deletions, and structural variants is an established method used to investigate the genetic causes and associations of disease. While whole genome and whole exome sequencing is a highly cost-effective and versatile method that assays gene sequence thus yielding both genetic and functional information. We, therefore, developed GeneTarget, a clinical genetic framework for the clinical trials analysis and interpretation of DNA sequencing data. The software is designed for use by clinicians and other users without an in-depth background in genetics.


##  Implementation
GeneTarget is available on GitHub https://github.com/collaborativebioinformatics/directed_sv_annotation. The repository provides detailed instructions for tool usage and installation. A bash script for an automated installation of the required dependencies.


##  Operation
The workflow of our tool is described as follows:
As an initial step, the user will have the option to choose a disease from a list of neurological conditions. Once this is done, a list of genes known to be associated with the chosen disease is generated. In parallel,  NGs are also required as inputs in order to generate a BAM alignment file, which is then used to generate a VCF file using a specific SV detection method. Subsequently, a filtering step is included, so only the SVs that are in the genes list are included. Provided that this intersection shows results, this step triggers the downstream pipeline.
The downstream pipeline starts with the labelling of clinical trial data, where a sample of individuals is selected and classified according to a treatment group (placebo/treatment). Next, tabular data regarding structural variant events are collected for all individuals. The latter are then used as input for the survival analysis step, which is performed on each of the treatment groups. 

##  Flowchart

<img src="https://github.com/collaborativebioinformatics/GeneTarget/blob/main/img/GeneTargetWorkflow.svg" width="700">

# Shiny App

## Input

![tab1](https://user-images.githubusercontent.com/73958439/195362195-b7dade92-be11-4a8b-b4a5-b4663cdbd6f5.PNG)


## Output

![image](https://user-images.githubusercontent.com/73958439/195366937-82edb5cb-92d2-4853-9a76-db49c596cd1d.png)
# Team

* Ahmad Al Khleifat

* Thomas Krannich

* Hiba Ben Aribi

* Marina Herrera Sarrias

* Moustafa Shokrof
