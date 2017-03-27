# ComBatHarmonization
### Multi-site harmonization with ComBat for imaging data

--------
**Maintainer**: Jean-Philippe Fortin, fortin946@gmail.com

**References**: If you are using ComBat for the harmonization of multi-site imaging data, please cite the following two papers:

|       | Citation     | Paper Link
| -------------  | -------------  | -------------  |
| ComBat for multi-site DTI data    | Jean-Philippe Fortin, Drew Parker, Birkan Tunc, Takanori Watanabe, Mark A Elliott, Kosha Ruparel, David R Roalf, Theodore D Satterthwaite, Ruben C Gur, Raquel E Gur, Robert T Schultz, Ragini Verma, Russell T Shinohara. **Harmonization Of Multi-Site Diffusion Tensor Imaging Data**. bioRxiv, 2017  |[Link](http://biorxiv.org/content/early/2017/03/22/116541)| 
| Original ComBat paper for gene expression array    |  W. Evan Johnson and Cheng Li, **Adjusting batch effects in microarray expression data using empirical Bayes methods**. Biostatistics, 8(1):118-127, 2007.      | [Link](https://academic.oup.com/biostatistics/article/8/1/118/252073/Adjusting-batch-effects-in-microarray-expression) |


## Table of content
- [1. Introduction](#id-section1)
- [2. Software](#id-section2)

<div id='id-section1'/>

## 1. Introduction



RAVEL is an R package that combines the preprocessing and statistical analysis of magnetic resonance imaging (MRI) datasets within one framework. Users can start with raw images in the NIfTI format, and end up with a variety of statistical results associated with voxels and regions of interest (ROI) in the brain. RAVEL stands for _Removal of Artificial Voxel Effect by Linear regression_, the main preprocessing function of the package that allows an effective removal of between-scan unwanted variation. We have shown in [a recent paper](http://www.sciencedirect.com/science/article/pii/S1053811916001452) that RAVEL improves significantly population-wide statistical inference. The vignette is divided into several sections. In Section 1, we present a pre-normalization preprocessing pipeline from raw images to processed images ready for intensity normalization. In Section 2, we explain how to use the RAVEL algorithm as well as other intensity normalization techniques. In Section 3, we present different tools for post-normalization statistical analysis. In Section 4, we present additional functions that help the visualization of images and statistical results. 


<div id='id-section2'/>

## 2. Software

The reference implementation of ComBat is written in R and is part of the `sva` package available through the Bioconductor project [here](https://bioconductor.org/packages/release/bioc/html/sva.html). We include here a reimplementation of ComBat in both R and Matlab for the harmonization of imaging data. Our implementation extends the original code for more flexibility and better visualization of the internal components of the algorithm. We are also currently working on several extensions of the original method that will be included here as well. 





