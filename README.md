# ds_practicum_project

Data Science Practicum Project for completion of the MS in Data Science, expected December 2023

This project explores the application of machine learning methods for analyzing coral algae and bacteria relationships, including Principal Components Analysis, K-Means, and classification algorithms. Traditional bioinformatics methods are well-documented, such as the R libraries of 'phyloseq', 'vegan', and many others. The application of machine learning methods is novel in the coral microbiome research community. The scope of this project involves an exploration of how machine learning methods may be applied; therefore, the focus is to understand the application and usage of the above-mentioned methods on data collected under the March 2023 publication. 

Note: Some function calls take a very long time to run, namely the K-means clustering in the files referencing "coseq". 

Note: Some additional work for a different course (Data 642) is included as the client permitted the use of the coral data for projects in both courses. The goals of each course's projects are different. 

In Data 793 (main directory with ```analysis``` folder  ```.Rmd``` files) contains work related to K-means clustering and binary classification of Clade C vs not Clade C. This project is in R. 

The Data 642 work contains a separate sub-directory (```data_642_jupyter_notebooks```) where the project is in Python with Jupyter Notebooks associated with modeling binary classification for Clade A v. Clade C. Clade A is the most dominant clade of the coral data, and as such, the underlying dataset used is different to allow for the max number of samples that contain Clade A sequencing. 


# R Version

R version 4.3.1 (2023-06-16) -- "Beagle Scouts"

# R Packages & Versions - to be revised

tidyverse

stats

factoextra

janitor

leaflet

viridis (?)

plotly

ggfortify

Rtsne

coseq

cluster (?)



# RStudio Version

Version 2023.09.0+463 (2023.09.0+463)

# Operating System

Mac OSX Ventura 13.5.2 (22G91)




