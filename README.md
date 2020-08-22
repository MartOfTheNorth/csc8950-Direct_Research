# csc8950-Direct_Research:Features analyses to treatment in mental disorders with machine learning


## Reseach paper collection
[https://github.com/MartOfTheNorth/Brain_Space_Initiative](https://github.com/MartOfTheNorth/Brain_Space_Initiative)

## Contents
### Part 1 : Abstract       
### Part 2 : Introduction
### Part 3 : Experiment     
### Part 4 : Results
### Part 5 : Conclusions

# Part 1 - Abstract



# Part 2 - Introduction


## Part 2.1 Literature Review
### Part 2.1.1. Combining fMRI and SNP data to investigate connections between brain function and genetics using parallel ICA.

Citation:  Liu J, Pearlson G, Windemuth A, Ruano G, Perrone-Bizzozero NI, Calhoun V. Combining fMRI and SNP data to investigate connections between brain function and genetics using parallel ICA. Hum Brain Mapp. 2009;30:241–255. https://onlinelibrary.wiley.com/doi/full/10.1002/hbm.20508

#### Goal: To link the genomic fators to brain functions.
#### Solve: 
- 1) Revealing brain functions from fMRI
- 2) Identifying genetic influences from SNP data
- 3) Finding relationship between brain functions and genetics.
#### Methodology: 
##### Parallel Independent Component Analysis (Parallel ICA). The common ICA is used in many reseaches to reveal factors without prior knowledge of the factor properties. Principle Component Analysis (PCA) is always used before proceeding ICA because of its advancetage to reduce the dimension of matrix.
###### ICA
- <img src="http://latex.codecogs.com/gif.latex?X=A$\cdot$S; Z=W\cdotX;" border="0" />
- <img src="http://latex.codecogs.com/gif.latex?If  W=A^{-1}, then Z=S;" border="0" />
###### Maximization;
- <img src="http://latex.codecogs.com/gif.latex?max\{H(Y)\}=-E[\ln{f_y}(Y)];" border="0" />
- <img src="http://latex.codecogs.com/gif.latex?Y=\frac{1}{1+e^{-U}}," border="0" />
- <img src="http://latex.codecogs.com/gif.latex?U=W$\cdot$X+W_0" border="0" />
- where f_y(Y) is the probability density function of Y. E is the expected value. H is the entropy function.
##### Parallel ICA Structure
- Paralled ICA is to solve all three objectives simultaneously.
- <img src="http://latex.codecogs.com/gif.latex?Corr(A_{1i},A_{2j}=\frac{Cov(A_{1i},A_{2j})}{Std(A_{1i})Std(A_{2j})};" border="0" />
- <img src="http://latex.codecogs.com/gif.latex?A_1=W_1^{-1};" border="0" />
- where Corr is the correlation function; Cov is the covariance function. Std is the standard deviation function. i and j are indices of components.
#### Result
- Parallel ICA has shown a correlation of 0.38 between one fMRI component and one genetic component.
#### Analysis and Discussion
- There is relationship between fMRI and genetic data.

### Part 2.1.2. Translational Potential of Neuroimaging Genomic Analyses to Diagnosis and Treatment in Mental Disorders.

Citation: J. Chen, J. Liu and V. D. Calhoun, "Translational Potential of Neuroimaging Genomic Analyses to Diagnosis and Treatment in Mental Disorders," in Proceedings of the IEEE, vol. 107, no. 5, pp. 912-927, May 2019. doi: 10.1109/JPROC.2019.2913145 https://ieeexplore.ieee.org/document/8710364

#### Goal: Review of "Genotypes and Phenotypes" in imaging genetics.
#### Solve: Observing the analysis strategies in imaging genetics. Groping them into 4 categories and reviewing "multivariate analysis methods" of each categories.
#### Methodology: 
##### Category 1:Candidate genotype with candidate phenotype.
- Univariate Analyses;
##### Category 2:Sets of genotypes with candidate phenotype.
- Univariate analyses with correction;
-   GSEA
-   GRS
-   MDR
-   PCA
-   ICA
-   Clustering
##### Category 3:Candidate genotype with multiple imaging phenotypes.
- Voxel-wise analyses with correction;
-   ICA
-   Group-ICA
-   Tensor-ICA
-   IVA
##### Category 4:Sets of genotypes with multiple imaging phenotypes.
- Mass Univariate Linear Model (MULM);
-   PLS
-   CCA
-   RRR
-   Parallel ICA

#### Analysis and Discussion (Challenge and Future Developments)
- Future reseach of imaging genetics is expected to increase and to include wide scale of multiple level studies.

### Part 2.1.3. A review of multivariate analyses in imaging genetics.

Citation: Liu J and Calhoun VD (2014) A review of multivariate analyses in imaging genetics. Front. Neuroinform. 8:29. doi: 10.3389/fninf.2014.00029 
https://www.frontiersin.org/articles/10.3389/fninf.2014.00029/full

#### Goal: 
#### Solve: 
- 
#### Methodology: 
##### 

#### Result
#### Analysis and Discussion

### Part 2.1.4. Brain Imaging Genomics: Integrated Analysis and Machine Learning.

Citation: L. Shen and P. M. Thompson, "Brain Imaging Genomics: Integrated Analysis and Machine Learning," in Proceedings of the IEEE, vol. 108, no. 1, pp. 125-162, Jan. 2020. 
https://ieeexplore.ieee.org/abstract/document/8886705

#### Goal: 
#### Solve: 
- 
#### Methodology: 
##### 

#### Result
#### Analysis and Discussion

### Part 2.1.5. COINSTAC: A Privacy Enabled Model and Prototype for Leveraging and Processing Decentralized Brain Imaging Data.

Citation: Plis SM, Sarwate AD, Wood D, Dieringer C, Landis D, Reed C, Panta SR, Turner JA, Shoemaker JM, Carter KW, Thompson P, Hutchison K and Calhoun VD (2016) COINSTAC: A Privacy Enabled Model and Prototype for Leveraging and Processing Decentralized Brain Imaging Data. Front. Neurosci. 10:365. doi: 10.3389/fnins.2016.00365
https://www.frontiersin.org/articles/10.3389/fnins.2016.00365/full

#### Goal: To solve the privacy limitation of data sharing.
#### Solve: Purpose COINSTAC platform which is dynamic decentralized platform.  
- COINSTAC does fill missing data.
- Pooling opened/closed data from multiple repositories.
- Enable destributed computation.

#### Methodology: 
##### For decentralized accoumplishment, COINSTAC has combined 3 existing frameworks; ViPAR, ENIGMA, and dataSHIELD in one platform.

###### 2.1.5.1 ViPAR (Virtual Pooling and Analysis of Research data): Pull subset data to trusted centralized server via encrypted link.
####### Limitation: No privacy on data.

###### 2.1.5.2 ENIGMA (Enhancing Neuroimaging Genetics Through Meta Analysis): Sharing summary statistics from local data.
####### Limitation: Time consuming due to many manuale processes. Single shot (comparing to iterate among sites).

###### 2.1.5.3 dataSHIELD : Decentralized data control (More privacy control) 
####### Limitation: No privacy on data.

###### 2.1.5.4 Beacons : Decentralized data sharing via web based tool. 
####### Limitation: No privacy on data.



#### Result
#### Analysis and Discussion


### Part 2.1.6. Decentralized Analysis of Brain Imaging Data: Voxel-Based Morphometry and Dynamic Functional Network Connectivity.

Citation: Gazula H, Baker BT, Damaraju E, Plis SM, Panta SR, Silva RF and Calhoun VD (2018) Decentralized Analysis of Brain Imaging Data: Voxel-Based Morphometry and Dynamic Functional Network Connectivity. Front. Neuroinform. 12:55. doi: 10.3389/fninf.2018.00055 
https://www.frontiersin.org/articles/10.3389/fninf.2018.00055/full

#### Goal: 
#### Solve: 
- 
#### Methodology: 
##### 

#### Result
#### Analysis and Discussion


### Part 2.1.7. Sharing privacy-sensitive access to neuroimaging and genetics data: a review and preliminary validation.

Citation: Sarwate AD, Plis SM, Turner JA, Arbabshirani MR and Calhoun VD (2014) Sharing privacy-sensitive access to neuroimaging and genetics data: a review and preliminary validation. Front. Neuroinform. 8:35. doi: 10.3389/fninf.2014.00035
https://www.frontiersin.org/articles/10.3389/fninf.2014.00035/full

#### Goal: 
#### Solve: 
- 
#### Methodology: 
##### 

#### Result
#### Analysis and Discussion

# Part 3 - Experiment

# Part 4 - Results

# Part 5 - Conclusions


