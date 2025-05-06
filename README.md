# Statistical Analysis Repository

This repository contains Jupyter notebooks for performing various statistical analyses, with two main branches: **distributions** and **inferential_statistics**. Each branch focuses on different aspects of statistical theory and practice.

## Branches

### 1. `distributions` Branch
The `distributions` branch includes Jupyter notebooks that demonstrate how to work with various probability distributions and visualize them. These notebooks provide both the theoretical background and practical code for calculating probability density functions (PDFs), cumulative distribution functions (CDFs), and generating plots.

#### Notebooks in the `distributions` Branch:
- **Exponential Distribution**: Understanding and visualizing the exponential distribution, including calculation of mean, variance, and percentile values.
- **Gamma Distribution**: Calculation and plotting of the gamma distribution’s PDF and its properties like mean, variance, etc.
- **Beta Distribution**: Exploration of the beta distribution with examples, including mean, variance, and mode calculations.

### 2. `inferential_statistics` Branch
The `inferential_statistics` branch contains Jupyter notebooks for performing inferential statistical analysis, such as detecting outliers using the Interquartile Range (IQR) and Z-Score methods, and conducting a Z-Test for hypothesis testing.

#### Notebooks in the `inferential_statistics` Branch:
- **Outliers Detection Using IQR**: The Interquartile Range method for detecting outliers in a dataset by identifying values outside the bounds defined by \(Q1 - 1.5 \times IQR\) and \(Q3 + 1.5 \times IQR\).
- **Outliers Detection Using Z-Score**: The Z-score method for detecting outliers based on how many standard deviations a data point is from the mean. Any point with an absolute Z-score greater than a defined threshold (commonly 3) is considered an outlier.
- **Z-Test**: A statistical test for hypothesis testing that compares a sample mean to a population mean. The Z-test is used to determine whether the sample mean is significantly different from the population mean.

## How to Use

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your-username/your-repository-name.git
