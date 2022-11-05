library(Rcpp)
Rcpp::sourceCpp("mySweep_cpp.cpp")


start <- Sys.time()
set.seed(123)
X <- rnorm(50000)
dim(X)<-c(100,500)
n <- nrow(X)
p <- ncol(X)
A = t(X)%*%X
mySweep_cpp(A,p)
end <- Sys.time()
elapse <- end - start
print(elapse)

