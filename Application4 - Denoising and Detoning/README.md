# ML-for-Asset-Manager

Implementation of code snippets and exercises from [Machine Learning for Asset Managers (Elements in Quantitative Finance)](https://www.amazon.com/Machine-Learning-Managers-Elements-Quantitative/dp/1108792898)
written by Prof. Marcos López de Prado.

## Chapter 2 Denoising and Detoning

Marcenko-Pasture theoretical probability density function, and empirical density function:
| ![marcenko-pastur.png](https://github.com/michaelsyao/ML-for-Asset-Manager/blob/main/img/gaussian_mp.png) | 
|:--:| 
| *Figure 2.1:Marcenko-Pasture theoretical probability density function, and empirical density function:* |

https://github.com/michaelsyao/ML-for-Asset-Manager/blob/main/img/gaussian_mp.png

Denoising a random matrix with signal using the constant residual eigenvalue method. This is done by fixing random eigenvalues. See code snippet 2.5
| ![eigenvalue_method.png](https://github.com/michaelsyao/ML-for-Asset-Manager/blob/main/img/figure_2_3_eigenvalue_method.png) | 
|:--:| 
| *Figure 2.2: A comparison of eigenvalues before and after applying the residual eigenvalue method:* |

Detoned covariance matrix can be used to calculate minimum variance portfolio. The efficient frontier is the upper portion of the minimum variance frontier starting at the minimum variance portfolio. A denoised covariance matrix is less unstable to change.

Note: Excersize 2.7: "Extend function fitKDE in code snippet 2.2, so that it estimates through
cross-validation the optimal value of bWidth (bandwidth)".
