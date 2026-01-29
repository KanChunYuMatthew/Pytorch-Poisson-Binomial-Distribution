# Pytorch-Poisson-Binomial-Distribution

## Meeting (Jan 29, 2026)

- Develop exact Poisson-binomial distribution `PoissonBinomial` using `dp` and `fft`
  - Test the sampling; to make sure the function is correct.
  - Numerical quantile: algo? `scipy.stats` used `optimize.brentq`; or you can use Newton methods
  - QQ plot
- Develop alternative approx distribution to `PoissonBinomial`
  - `RefinedNormalPB`: mean, variance, quantile
  - ...
  - Tests


## References
- [On computing the distribution function for the Poisson binomial distribution](https://www.sciencedirect.com/science/article/pii/S0167947312003568)
- [cupy](https://cupy.dev/)
- [cuML](https://docs.rapids.ai/api/cuml/stable/)