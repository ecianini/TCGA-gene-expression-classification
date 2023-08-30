# TCGA-gene-expression-classification

Project for the Scientific Programming course of "Bioinformatics for Computational Genomics" MSc.

The notebook can be visualized [here](https://nbviewer.org/github/ecianini/TCGA-gene-expression-classification/blob/main/Scientific_Programming_Project.ipynb).

## Aim 
In this work several machine learning' classification techniques were applied on the breast invasive carcinoma gene expression data coming from the Cancer Genome Atlas Program ([TCGA](https://www.cancer.gov/ccg/research/genome-sequencing/tcga)) downloaded from the [GenoSurf](http://geco.deib.polimi.it/genosurf/) interface.

The aim of the project was to predict the status of the patients (healthy vs tumoral) based on the gene expression values taking advantage of some of the most popular machine learning algorithms. 


## Dataset description
The GenoSurf interface was used to download the related data, selecting as options:

* project_name: ['tcga-brca']
* assembly: ['grch38']
* data_type: ['gene expression quantification']
* is_healthy:
  - ['false'] for tumoral data
  - [true] for normal data.
 
## Outline 
Once downloaded, to reduce the complexity of the dataset, filtering methods such as the *Principal Component Analysis* for *feature selection* were applied to the data.

Then, the 6 canonical classification algorithms were used to train the classification models:
* Logistic Regression
* SVC with linear kernel
* SVC with polynomial kernel
* K-nearest Neighbours
* Linear Discriminant Analysis
* Quadratic Discriminant Analysis

To better evaluate the models, a k-fold cross-validation (k = 10) was performed and the hyper-parameter tuning of the best models was made to maximize the accuracy.







