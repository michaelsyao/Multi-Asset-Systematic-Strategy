# Hierarchical Risk Parity and Clustering Application
```
This section forcuses on Clustering application on Portfolio Allocation 
```
## A. Hierarchy Risk Parity
#### The Problem With Markwoitz's Optimization Method
>  The more correlated the investments, the greater the need for diversification, and yet the more likely we will receive unstable solutions. The benefits of diversification often are more than offset by estimation errors.
#### From Geometric to Hierarchical Relationships
> Suppose that an investor wishes to build a diversified portfolio of securities, including hundreds of stocks, bonds and hedge fund, real estate, private placemnets and etc. Some investments seem closer substitutes for one another, and ohter investments seem complementary to one another.
> Yet, to a correlation matrix all investments are potential substitutes to one another. In other words correlation matrices lack the notion of hierarchy. This lack of hierarchical structure allowes weights to vary freely in unintended ways, which is a root cause of Critical Line Algorithm (CLA)'s instability.
#### A tree structure introduces 2 desirable features
> 1. It has only N-a edges to connect N nodes, so the weights only reblances among peers are various hierarchical levels.
> 2. The weights are distributed top-down, consistent with how many asset managers build their portfolios, such as from asset class to sectors to individual securities.
#### Summary
> The author is saying that this full tree has no hierarchy, but in really portfolio allocation, hierarchy is needed. For example, if I am aollocating in financials, consumer staples and tech, each of these sectors have some correlations, equties within those sectors have correlations among themselves. So, the author is proposing a hierarchical tree structure instead of a matrix.

> The Hierarchical Risk Parity method uses the information contained in the covariance matrix without requiring its inversion or positive-definitiveness. The algorithm operates in 2 stages 1) tree clustering 2) qusai-diagonalization, 3) recursive bisection.

1. [HierarchicalRiskParity](https://github.com/michaelsyao/Multi-Asset-Systematic-Strategy/blob/main/SectionA.Portfolio%20Construction/01.PF_Hierarchical%20Risk%20Parity.ipynb)

## B. Eigen-portfolio construction using Principal Component Analysis (PCA)
> Use Eigen-portfolio construction using PCA method
1. [Eigen Portfolio PCA](https://github.com/michaelsyao/Multi-Asset-Systematic-Strategy/blob/main/SectionA.Portfolio%20Construction/02.PF_Eigen.PCA.ipynb)

## C. Use Eigen for Denoised portfolio
> Use Eigen for Denoised portfolio
2. [Eigen for Denoised PF](https://github.com/michaelsyao/Multi-Asset-Systematic-Strategy/blob/main/SectionA.Portfolio%20Construction/03.PF_Denoised_Eigen_value.py)
