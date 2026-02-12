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

## Meeting (Feb 12, 2026)

- Todo items in the last meeting
- **Sufficient and series** Benchmarking the exact and approx methods
  - Time complexity (running time)
  - TAE of the approx and exact methods: PMF and quantiles
  - recommendation of the use cases for the exact and approx methods - default arguments for the `PoissonBinomial` class
- implement `expand` for `PoissonBinomial` class;
  - Understand the `expand` method in PyTorch; such as `Binomial` <https://github.com/pytorch/pytorch/blob/v2.10.0/torch/distributions/binomial.py#L24>
  - Implement `expand` for `PoissonBinomial` class;
  - Testing; example for real application

## References
- [On computing the distribution function for the Poisson binomial distribution](https://www.sciencedirect.com/science/article/pii/S0167947312003568)
- [cupy](https://cupy.dev/)
- [cuML](https://docs.rapids.ai/api/cuml/stable/)