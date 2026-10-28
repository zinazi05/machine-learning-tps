# ML Lab Session 2 — Part A: PCA from scratch

**What I did.** Implemented Principal Component Analysis with only pandas and NumPy on the grades of six students in four subjects (Mathematics, Statistics, Programming, Algorithms):
1. Loaded the data into a DataFrame and displayed its dimensions and descriptive statistics.
2. Standardized the variables (mean and standard deviation).
3. Computed the covariance matrix of the standardized data.
4. Computed its eigenvalues and eigenvectors with NumPy.
5. Sorted them in descending order of eigenvalue and kept the two largest components.
6. Projected the data onto those two components.
7. Computed the explained variance ratio of each component and the cumulative explained variance.

**Benefit.** Shows how PCA works step by step: the principal components are the eigenvectors of the covariance matrix, and their eigenvalues measure how much variance each one captures. It also reduces four correlated variables to two components while keeping most of the information, and gives the reference results that Part B (scikit-learn) is compared against.