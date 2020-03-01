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
### 1. Liu J, Pearlson G, Windemuth A, Ruano G, Perrone-Bizzozero NI, Calhoun V. Combining fMRI and SNP data to investigate connections between brain function and genetics using parallel ICA. Hum Brain Mapp. 2009;30:241–255. https://onlinelibrary.wiley.com/doi/full/10.1002/hbm.20508

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
- <img src="http://latex.codecogs.com/gif.latex?Corr(A_{1i}, A_{2j}=\frac{Cov(A_{1i}, A_{2j})}{Std(A_{1i})\cdot Std(A_{2j})};" border="0" />

# Part 3 - Experiment

# Part 4 - Results

# Part 5 - Conclusions


