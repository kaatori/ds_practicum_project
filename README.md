# ds_practicum_project: Data Science Practicum Project

Data 793: Data Science Practicum Project for completion of the MS in Data Science, American University, Washington, D.C., December 2023.

This project explores the application of machine learning methods for analyzing coral algae and bacteria relationships, including Principal Components Analysis, K-Means, and classification algorithms. Traditional bioinformatics methods are well-documented, such as the R libraries of 'phyloseq', 'vegan', and many others. The application of machine learning methods is novel in the coral microbiome research community. The scope of this project involves an exploration of how machine learning methods may be applied; therefore, the focus is to understand the application and usage of the above-mentioned methods on data collected under the March 2023 publication. 

Note: Some function calls take a very long time to run, namely the K-means clustering in the files referencing "coseq" in the title. 

Note: Some additional work for a different course (Data 642) is included as the client permitted the use of the coral data for projects in both courses. The goals of each course's projects are different. 

In Data 793 (main directory with ```analysis``` folder  ```.Rmd``` files) contains work related to K-means clustering and binary classification of Clade C vs not Clade C. This project is in R. 

The Data 642 work contains a separate sub-directory (```data_642_jupyter_notebooks```) where the project is in Python with Jupyter Notebooks associated with modeling binary classification for Clade A v. Clade C. Clade A is the most dominant clade of the coral data, and as such, the underlying dataset used is different to allow for the max number of samples that contain Clade A sequencing. 


# Operating System

macOS Sonoma 14.1.2 (23B92)

# R Version

R version 4.3.1 (2023-06-16) -- "Beagle Scouts"

# RStudio Version

Version 2023.09.0+463 (2023.09.0+463)

# R Packages 

compositions 
corrplot 
coseq 
factoextra 
gbm
glmnet 
leaflet 
plotly 
randomForest  
Rtsne 
stats 
tidyverse 
tsne 
viridis 

# Overview of ```analysis``` folder (in ABC order): 

 [1] "./CLR.Rmd"   
 - Create centered log ratio (CLR) data transformations during initial testing. See also files used in the final stretch of the project that contain 'final' in the title.
 
 [2] "./Coseq_P.Rmd"      
 - K-means clustering of the Species P subset using the ```coseq``` library used in final report.
 
 [3] "./Coseq_S.Rmd"     
 -  - K-means clustering of the Species S subset using the ```coseq``` library used in final report.

 [4] "./Data_Split_Species.Rmd"  
 - Create the subsets of data by species used in initial parts of the analysis.
 
 [5] "./EDA_Bacteria ASV Table EDA.Rmd"   
 - EDA of the bacteria data from the client. 
 
 [6] "./EDA_Coral_Data_EDA.Rmd"      
 - EDA of the combined coral data with both algae and bacteria joined.
 
 [7] "./EDA_Coseq_EDA.Rmd"     
 - EDA of how the ```coseq``` library works, in particular the ```coseq()``` function which has the implementation of K-means for compositional data. 
 
 [8] "./Final_Correlation_Plots_Clustering_Analysis_Ridge_Lasso_ Best_Predictors.Rmd"
 - Correlation plots used for EDA as well as tying together the Part I (Unsupervised) clustering results with Part II (Supervised) modeling analysis. 
 
 [9] "./Final_Modeling_Clustering_Final_Analysis.Rmd" 
 - Analyzing the big picture of how the clustering assignments look when joined by the name of the ASV predictors from the modeling process. 
 - Used in final report. 
 
[10] "./Final_Ridge_Lasso_Modeling_Revised.Rmd"      
- Final modeling process for obtaining the error rates listed in the final report.

[11] "./Final_Tree_Methods_Clade_C.Rmd"   
- Final modeling process for the RandomForest and Boosted Trees models listed in final report.

[12] "./ITS2_Table.Rmd"  
- EDA of the Algae abundance counts from the client. 

[13] "./Jacard.Rmd"                   
- Code for computing the Jaccard Index for guaging the level of similarity (consistency) among cluster assignments across the 6 runs of K-means (3 for each species) used in final report. 

[14] "./Join.Rmd"    
- Process of joining the bacteria ASV columns with the algae information by the ```sample_id``` column. 

[15] "./Metadata_EDA.Rmd"    
- EDA of the metadata table from the client. 

[16] "./PCA_Clade_A.Rmd"   
- Added as an extra for the client to have PCA for Clade A for later review (not included in report as project focused on Clade C). 

[17] "./PCA_CLR.Rmd"   
- Initial runs of Principal Components Analysis (PCA) were by species before the focus of the project was on Clade C. Scroll down to obtain the PCA on Clade C, particularly the plot of the 'plateau' of there being approximately 150 (ish) ASVs that relatively evenly contribute to Clade C. 

[18] "./Testing_Experimental_Logistic_Regression_Clade_C.Rmd"      
- Sampling the balanced dataset of Clade C and non-Clade C to obtain the 278 rows balanced dataset. 
- The rest of the file is not really used in final analysis except as a step along in the process of refining the modeling. This file was to test the behavior and settings of the different ways to do logistic modeling with different libraries. 

[19] "./Testing_Logistic_Regression_Clade_C_Testing.Rmd"   
- Not used in final analysis. This was to test the behavior and settings of the different ways to do logistic modeling with different libraries. 

[20] "./Testing_RandomForest_Testing.Rmd"      
- Not used in final analysis. This was to test the behavior and settings for the modeling process. 

[21] "./Testing_Ridge_Lasso_Modeling_Testing.Rmd" 
- Not used in final analysis. This was to test the behavior and settings for the modeling process. 




