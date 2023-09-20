# VariantSurvival: A tool to identify genotype-treatment response
<img src="https://user-images.githubusercontent.com/41301333/195215088-8404f200-8297-4322-a30f-c84f526aa620.png" width="200" height="200" align="right">

### Table of Contents
1. [VariantSurvival](#variantsurvival)
2. [The shiny app](#the-shiny-app)
3. [The developers team](#the-developers-team)
<br>


## VariantSurvival
We present VariantSurvival, a lightweight application to visualize genotype-treatment response.
Its dashboard provides full functionality to import VCF data, tabular metadata as well as to select neurological diseases and target genes.
<br><br>
<img src="https://github.com/collaborativebioinformatics/VariantSurvival/blob/main/img/VariantSurvival.svg">


## The shiny app
The VariantSurvival Shiny application is implemented as an R package. Available [_here_](https://github.com/collaborativebioinformatics/VariantSurvival/tree/main/VariantSurvival_package).


### Installation
The package can be installed in R studio using the following command:

```
#install.packages('devtools') #install devtools package
library(devtools)
devtools::install_github("collaborativebioinformatics/VariantSurvival/VariantSurvival_package")
```
Note: All required packages will be installed automatically when installing "VariantSurvival".


### Running the demo
Follow these steps to run the VariantSurvival demonstration:

  1. Clone the Repository: Open your terminal and navigate to the directory where you want to clone the repository. Run the following command to clone the repository:
     
  ```
  git clone https://github.com/collaborativebioinformatics/VariantSurvival.git
  ```
  
  2. Set Working Directory: Change your current working directory to the _VariantSurvival_package/R/_ subfolder within the cloned repository.
     
  3. Run the Demonstration: Launch R in your terminal or RStudio, and execute the following command to run the demonstration:
  
  ```
  library(VariantSurvival)
  VariantSurvival::VariantSurvival(demo=TRUE)
  ```


### Running your data analysis
Details on formatting your input data for VariantSurvival: [VCF file](https://github.com/collaborativebioinformatics/VariantSurvival/blob/main/docs/preprocessing/prepareVCF.md), study groups metadata

VariantSurvival run example:
```
library(VariantSurvival)
VariantSurvival::VariantSurvival(vcffile="variant_file_.vcf", metadatafile= "metadata_file.xlsx")
```


## The developers team

* Ahmad Al Khleifat [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/AhmadAlKhleifat.svg?style=social&label=Follow%20%40AhmadAlKhleifat)](https://twitter.com/AhmadAlKhleifat)
* Thomas Krannich [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/krannich479.svg?style=social&label=Follow%20%40krannich479)](https://twitter.com/krannich479)
* Hiba Ben Aribi [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/Hiba_BenAribi.svg?style=social&label=Follow%20%40Hiba_BenAribi)](https://twitter.com/Hiba_BenAribi)
* Marina Herrera Sarrias
* Moustafa Shokrof [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/mostafashokrof2.svg?style=social&label=Follow%20%40mostafashokrof2)](https://twitter.com/mostafashokrof2)


