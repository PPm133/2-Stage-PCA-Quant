# 2-Stage-PCA-Quant
A very simple, naive implementation of the two-stage statistical factor model described in The Elements of Quantitative Investing (Paleologo 2024).
### Inputs
- **R**: Return matrix of shape (n, T), where:
  - `n` is the number of stocks.
  - `T` is the number of time periods.
- **tau_f, tau_s**: Exponential weighting decay factors.
- **p, m**: Dimensions to truncate the latent factors.

### Outputs
- **B**: Factor loading matrix of shape (n, m).
- **F**: Factor return matrix of shape (m, T).
- **Res**: Residual matrix of shape (n, T).

This model relies heavily on pre-processing and is sensitive to the hyperparameters. Also, this is a very naive approach and is only meant as a toy example.
