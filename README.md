# Inferential Statistics in Python

This repository contains Jupyter notebooks for performing various inferential statistical analyses, such as detecting outliers using the Interquartile Range (IQR) and Z-Score methods, and performing a Z-Test for hypothesis testing.

## Files in the `inferential_statistics` Subfolder

### 1. `OutliersIQR.ipynb`
This notebook demonstrates how to detect outliers in a dataset using the **Interquartile Range (IQR)** method. The steps are as follows:

- **Sort the Data**: The dataset is arranged in increasing order.
- **Calculate Quartiles**: The first (Q1) and third (Q3) quartiles of the dataset are computed.
- **IQR Calculation**: The Interquartile Range is calculated as \( IQR = Q3 - Q1 \).
- **Calculate Boundaries**: The lower and upper bounds are calculated as:
  - Lower Bound: \( Q1 - 1.5 \times IQR \)
  - Upper Bound: \( Q3 + 1.5 \times IQR \)
- **Outlier Detection**: Any values outside these bounds are considered outliers and removed from the dataset.

**How to Use**:
1. Input a dataset as a list of values.
2. The notebook calculates and prints the final dataset after outlier removal.
3. It also displays the detected outliers.

### 2. `OutliersZscore.ipynb`
This notebook demonstrates how to detect outliers using the **Z-Score** method. Z-scores measure how many standard deviations an element is from the mean. The steps are:

- **Calculate Mean and Standard Deviation**: The mean and standard deviation of the dataset are computed.
- **Calculate Z-Score**: The Z-score for each element is calculated as:
  \[
  Z = \frac{X - \mu}{\sigma}
  \]
  where \( \mu \) is the mean and \( \sigma \) is the standard deviation.
- **Outlier Detection**: Any value with an absolute Z-score greater than a defined threshold (commonly 3) is considered an outlier.

**How to Use**:
1. Input a dataset as a list of values.
2. The notebook calculates and prints the detected outliers based on the Z-score method.

### 3. `Ztest.ipynb`
This notebook demonstrates how to perform a **Z-Test** for hypothesis testing. A Z-test is used to compare the sample mean with the population mean when the standard deviation is known. The steps are:

- **State the Hypotheses**:
  - Null Hypothesis (\( H_0 \)): The sample mean is equal to the population mean.
  - Alternate Hypothesis (\( H_1 \)): The sample mean is not equal to the population mean.
  
- **Calculate Z-Score**: The Z-score is computed using the formula:
  \[
  Z = \frac{X - \mu}{\frac{\sigma}{\sqrt{n}}}
  \]
  where \( X \) is the sample mean, \( \mu \) is the population mean, \( \sigma \) is the population standard deviation, and \( n \) is the sample size.

- **Hypothesis Decision**: Based on the Z-score, we compare it with a critical value (e.g., 2.33 for a 99% confidence level) to either accept or reject the null hypothesis.

**How to Use**:
1. Input the sample mean, population mean, standard deviation, and sample size.
2. The notebook calculates the Z-score and helps you decide whether to accept or reject the null hypothesis.

---

## Dependencies

To run these notebooks, you will need the following Python packages:

- `numpy`
- `matplotlib`
- `scipy`

You can install the required dependencies using pip:

```bash
pip install numpy matplotlib scipy
