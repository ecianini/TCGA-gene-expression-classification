# TCGA-gene-expression-classification

Project for the Scientific Programming course of "Bioinformatics for Computational Genomics" MSc.

## Aim 
In this work several machine learning' classification techniques were applied on the breast invasive carcinoma gene expression data coming from the Cancer Genome Atlas Program ([TCGA](https://www.cancer.gov/ccg/research/genome-sequencing/tcga)) downloaded from the [GenoSurf](http://geco.deib.polimi.it/genosurf/) interface.

The aim of the project was to predict the status of the patients (healthy vs tumoral) based on the gene expression values, using some of the most popular machine learning algorithms. 


## Dataset description
The GenoSurf interface was used to download the related data, selecting as options:

* project_name: ['tcga-brca']
* assembly: ['grch38']
* data_type: ['gene expression quantification']
* is_healthy:
  - ['false'] for tumoral data
  - [true] for normal data.
 
## Outline 
Once downloaded, to reduce the complexity of the dataset 

