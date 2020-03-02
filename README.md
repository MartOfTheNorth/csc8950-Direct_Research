# csc8950-Direct_Research:Features analyses to treatment in mental disorders with machine learning


## Machine Learning reseach paper collection
[https://github.com/MartOfTheNorth/Panacea_Lab/wiki/Welcome-to-the-Panacea_Lab-wiki!](https://github.com/MartOfTheNorth/Panacea_Lab/wiki/Welcome-to-the-Panacea_Lab-wiki!)

## Contents
### Part 1 : Abstract       
### Part 2 : Introduction
### Part 3 : Experiment     
### Part 4 : Results
### Part 5 : Conclusions

# Part 1 - Abstract



# Part 2 - Introduction


## Part 2.1 Literature Review
### 2.1.1. Liu J, Pearlson G, Windemuth A, Ruano G, Perrone-Bizzozero NI, Calhoun V. Combining fMRI and SNP data to investigate connections between brain function and genetics using parallel ICA. Hum Brain Mapp. 2009;30:241–255. https://onlinelibrary.wiley.com/doi/full/10.1002/hbm.20508

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

### 2.1.2. J. Chen, J. Liu and V. D. Calhoun, "Translational Potential of Neuroimaging Genomic Analyses to Diagnosis and Treatment in Mental Disorders," in Proceedings of the IEEE, vol. 107, no. 5, pp. 912-927, May 2019. doi: 10.1109/JPROC.2019.2913145 https://ieeexplore.ieee.org/document/8710364

#### Goal: 
#### Solve: 
- 
#### Methodology: 
##### 

#### Result
#### Analysis and Discussion

### 2.1.3. Liu J and Calhoun VD (2014) A review of multivariate analyses in imaging genetics. Front. Neuroinform. 8:29. doi: 10.3389/fninf.2014.00029 
https://www.frontiersin.org/articles/10.3389/fninf.2014.00029/full

#### Goal: 
#### Solve: 
- 
#### Methodology: 
##### 

#### Result
#### Analysis and Discussion

### 2.1.4. L. Shen and P. M. Thompson, "Brain Imaging Genomics: Integrated Analysis and Machine Learning," in Proceedings of the IEEE, vol. 108, no. 1, pp. 125-162, Jan. 2020. 
https://ieeexplore.ieee.org/abstract/document/8886705

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


