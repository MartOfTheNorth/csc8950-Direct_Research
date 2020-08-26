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


### Part 2.1.5. Sharing privacy-sensitive access to neuroimaging and genetics data: a review and preliminary validation.

Citation: Sarwate AD, Plis SM, Turner JA, Arbabshirani MR and Calhoun VD (2014) Sharing privacy-sensitive access to neuroimaging and genetics data: a review and preliminary validation. Front. Neuroinform. 8:35. doi: 10.3389/fninf.2014.00035
https://www.frontiersin.org/articles/10.3389/fninf.2014.00035/full

#### Goal: To review some literature on 1) differential privacy, 2) a measuring framework for privacy loss, and 3) demonstrating this framework. Describe how differential privacy is used in Neuroinformatics.

#### Problem: Breakdown the challenge of the current methods; de-identified (aka data anonymization) on what they are and why they are not considered privacy coverage.

#### Solve: Introduce differential privacy framework. 
-      Output h = Alg(D) ∈ ∉
-   Adding randomized approximation PrivAlg;
-      P (PrivAlg($D) ∈ S ≤ P (PrivAlg($D') ∈ S
-   Using laplace distribution as popolor method. There are also different methods.
##### Challenges of differential privacy framework.
- However adding this randomization to protect privacy, cost is the low accuracy. 
- Coming up with standard end-to-end differentially private analysis toolkits to allow allow researchers to write programs, for examples, PINQ (2010), Fuzz (2010), AIRAVAT (2010), or GUPT (2012).
#### Methodology: 
##### Perform statistical derivatives locally and share the differentially private data derivatives. Because of the injected noise causes, degradation of performance is noticable. The compomization of this challenge is to use large aggregation of large dataset. Paper demonstrated into two perspectives.
##### a) Estimating a mean (Laplace distribution)
##### b) Classification 
 <img src="https://www.frontiersin.org/files/Articles/79221/fninf-08-00035-HTML/image_m/fninf-08-00035-g001.jpg" border="0" />

#### Result
##### The Combined classifier of multiple sites clearly show the significant advantage over single local site.
 <img src="https://www.frontiersin.org/files/Articles/79221/fninf-08-00035-HTML/image_m/fninf-08-00035-g002.jpg" border="0" />

#### Analysis and Discussion
- Lack of DUAs would be compromised with differential privacy framework.
- Challenge of data sharing would need to be addressed in both policy and technology sides.

### Part 2.1.6. COINSTAC: A Privacy Enabled Model and Prototype for Leveraging and Processing Decentralized Brain Imaging Data.

Citation: Plis SM, Sarwate AD, Wood D, Dieringer C, Landis D, Reed C, Panta SR, Turner JA, Shoemaker JM, Carter KW, Thompson P, Hutchison K and Calhoun VD (2016) COINSTAC: A Privacy Enabled Model and Prototype for Leveraging and Processing Decentralized Brain Imaging Data. Front. Neurosci. 10:365. doi: 10.3389/fnins.2016.00365
https://www.frontiersin.org/articles/10.3389/fnins.2016.00365/full

#### Goal: To solve the privacy limitation of data sharing.

#### Problem: Current platforms with their limitation.
- ViPAR (Virtual Pooling and Analysis of Research data): Pull subset data to trusted centralized server via encrypted link.
##### Limitation: No privacy on data.

- ENIGMA (Enhancing Neuroimaging Genetics Through Meta Analysis): Sharing summary statistics from local data.
##### Limitation: Time consuming due to many manuale processes. Single shot (comparing to iterate among sites).

- dataSHIELD : Decentralized data control (More privacy control) 
##### Limitation: No privacy on data.

- Beacons : Decentralized data sharing via web based tool. 
##### Limitation: No privacy on data.

#### Solve: Purpose COINSTAC platform which is dynamic decentralized platform.  
- COINSTAC does fill missing data.
- Pooling opened/closed data from multiple repositories.
- Enable destributed computation.
- Convenient and powerful web-based platform

#### Methodology: 
##### COINSTAC Model : For decentralized accoumplishment, COINSTAC has combined 3 existing frameworks; ViPAR, ENIGMA, and dataSHIELD in one platform.
- Ease of Interaction and Collaboration
- Decentralized Algorithms
- Privacy Preserving Data Mining
- Web-based End-use Platform

 <img src="https://www.frontiersin.org/files/Articles/204805/fnins-10-00365-HTML/image_m/fnins-10-00365-g001.jpg" border="0" />

##### COINSTAC Algorithms : 

 <img src="https://www.frontiersin.org/files/Articles/204805/fnins-10-00365-HTML/image_m/fnins-10-00365-g002.jpg" border="0" />

#### Result
##### Test environments are set into two studies. Single-shot Vs Iterative. Using ridge regression model.
- Camparing the accuracy of classification:
-   Single-shot  : 0.061375
-   Iterative    : 0.061530
-   Centralized  : 0.061542
- The decentralized result (single-shot and ierative) is very close to the centralized result.

#### Analysis and Discussion
- The main benefit of COINSTAC is to cut time and process of DUI in each organization.
- COINSTAC is not required to share raw data by concept desgin while provides the end-goal reseach purpose.
- Provide ability to re-run and re-analisis quickly.
- Support all main OSs including mobile devices.
- COINSTAC meets all envision goals.



### Part 2.1.7. Decentralized Analysis of Brain Imaging Data: Voxel-Based Morphometry and Dynamic Functional Network Connectivity.

Citation: Gazula H, Baker BT, Damaraju E, Plis SM, Panta SR, Silva RF and Calhoun VD (2018) Decentralized Analysis of Brain Imaging Data: Voxel-Based Morphometry and Dynamic Functional Network Connectivity. Front. Neuroinform. 12:55. doi: 10.3389/fninf.2018.00055 
https://www.frontiersin.org/articles/10.3389/fninf.2018.00055/full

#### Goal: Purpose two decentralized algorithms; 
- 1) Decentralized regression algorithem for performing VBM (Voxel-Based Morphometry) on sMRI (structure Magnetic Resonance Imaging)
- 2) Decentralized dFNC (Dynamic Functional Network Connectivity) algorithem aka ddFNC in both;
##### Spatial ICA (Independent Component Aanlysis) aka dgICA.
##### K-Means aka dK-Means
- Compare those two decentralized algorithem with centralized algorithem (pooled data)

#### Solve: 
- ENIGMA (2017) and ViPAR (2015) allows locally data processing, however combining the meta-analysis results among mutlitple sites is challenge.
- To mention that COINSTAC (2016) has solution for this problem while using different algorithms.

#### Methodology: 
##### 

#### Result: Decentralized algorithms provide similar result as centralized in the same data.

#### Analysis and Discussion




# Part 3 - Experiment

# Part 4 - Results

# Part 5 - Conclusions


