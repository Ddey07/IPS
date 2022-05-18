# IPS
Iterative Proportional Scaling Algorithm in R

This code is a slight modification of the code in https://github.com/donaldmusgrove/thesis

Once you have set the working directory to the files in this repository, run the following: 

library(Rcpp)
Rcpp::sourceCpp('IPS2.cpp')
source('helper_function2.R')


The IPS function takes argument as your starting Positive Definite matrix S, an adjacency matrix A and eps (the thresholding of error)

K_ips = IPS(S=S, A= A, eps = 1e-8)

S_ips will be the precision matrix post-covariance selection with respect to the graph with adjacency matrix A. 


