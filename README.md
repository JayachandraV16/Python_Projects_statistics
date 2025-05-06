# Distribution Functions in Python

This repository contains Jupyter notebooks for exploring and visualizing three important probability distributions: **Exponential**, **Gamma**, and **Beta**. Each notebook includes code to calculate the probability density functions (PDFs) for these distributions, compute statistical properties (like mean and variance), and visualize the results with plots.

## Files in the `distribution` Subfolder

### 1. `Exponential_dist.ipynb`
This notebook demonstrates the **Exponential Distribution**, which is often used to model time between events in a Poisson process. It focuses on the following aspects:

- **Exponential PDF Calculation**: The notebook computes the probability density function for the exponential distribution using the formula:
  \[f(x; \beta) = \frac{1}{\beta} e^{-x/\beta}\]
  where \( \beta \) is the rate parameter (scale).
  
- **Expected Value and Variance**: Calculates the expected value \( E(x) = \frac{1}{\beta} \) and variance \( \text{Var}(x) = \frac{1}{\beta^2} \).
  
- **Visualization**: It plots the PDF of the exponential distribution, with shading under the curve and highlights for the mean and 95th percentile.

**How to Use**:  
- Input a value for `x` (the point where you want the PDF) and the parameter `β` (rate parameter).
- The notebook will calculate the PDF, mean, variance, and visualize the distribution.

### 2. `Gamma_dist.ipynb`
This notebook demonstrates the **Gamma Distribution**, which generalizes the exponential distribution. The Gamma distribution is frequently used in queuing theory and for modeling the waiting times of multiple events. Key features include:

- **Gamma PDF Calculation**: The notebook computes the PDF of the Gamma distribution using the formula:
  \[
  f(x; \alpha, \beta) = \frac{\beta^\alpha}{\Gamma(\alpha)} x^{\alpha - 1} e^{-x/\beta}
  \]
  where \( \alpha \) is the shape parameter and \( \beta \) is the scale parameter.
  
- **Expected Value and Variance**: Computes the expected value \( E(x) = \frac{\alpha}{\beta} \) and variance \( \text{Var}(x) = \frac{\alpha}{\beta^2} \).
  
- **Visualization**: Plots the Gamma distribution's PDF, showing the mean on the plot.

**How to Use**:  
- Input values for `x`, `α` (shape parameter), and `β` (scale parameter).
- The notebook will calculate the PDF, mean, variance, and display the plot.

### 3. `Beta_distribution.ipynb`
This notebook demonstrates the **Beta Distribution**, which is commonly used in Bayesian statistics, particularly when modeling probabilities in the interval [0, 1]. The Beta distribution is defined by two parameters \( \alpha \) and \( \beta \).

- **Beta PDF Calculation**: The notebook computes the Beta distribution's PDF using the formula:
  \[
  f(x; \alpha, \beta) = \frac{x^{\alpha - 1} (1 - x)^{\beta - 1}}{B(\alpha, \beta)}
  \]
  where \( B(\alpha, \beta) \) is the Beta function.
  
- **Expected Value and Variance**: Calculates the expected value \( E(x) = \frac{\alpha}{\alpha + \beta} \), and variance \( \text{Var}(x) = \frac{\alpha \beta}{(\alpha + \beta)^2 (\alpha + \beta + 1)} \).
  
- **Mode**: The mode (if it exists) is calculated using the formula:
  \[\text{Mode} = \frac{\alpha - 1}{\alpha + \beta - 2}\]
  for \( \alpha > 1 \) and \( \beta > 1 \).
  
- **Visualization**: Plots the Beta distribution's PDF with highlights for the mean and mode.

**How to Use**:  
- Input values for `α` and `β` (both shape parameters of the Beta distribution).
- The notebook will calculate the Beta PDF, mean, variance, mode (if applicable), and display the plot.


## Dependencies

To run these notebooks, you will need the following Python packages:

- `numpy`
- `matplotlib`
- `seaborn`
- `scipy`

You can install the required dependencies using pip:

```bash
pip install numpy matplotlib seaborn scipy
