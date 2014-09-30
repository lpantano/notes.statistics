# Modelling 
## Generalized linear models
this is a summary from the notes in this course (http://data.princeton.edu/wws509)

### the model

* We assume has a random structure
* We need to estimate the predictors beta and variation of data

### estimation

* The likelihood principle instructs us to pick the values of the parameters that maximize the likelihood, or equivalently, the logarithm of the likelihood function. If the sigma is fixed, this means minimizing residual sum of squares
* In this case beta doesn't depend on sigma, and is a global maximum.
*  the assumption of normality of the observations is required only for inference in small samples. 
* __The really important assumption is that the observations are uncorrelated and have constant variance__
* sigma can be estimated from beta: RSS(beta)/n-p to get unbiased variance.
*  under normality, RSS/sigma^2 has a chi-squared distrbituion with n-p d.f

```
y.lm <- lm(y~1)
n <- length(y)
sqrt(sum(abs(residuals(y.lm))^2)/99) == sd(y)
```
