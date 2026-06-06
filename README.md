# Volatility Surface Reconstruction

## Competition

FinClub Open Project 2

## Objective

Reconstruct missing implied volatility values in an options volatility surface.

## Dataset

- 975 timestamps
- 28 option contracts
- 5460 missing values

## Methodology

### Baseline

- Iterative Imputer (Bayesian Ridge)

Public Score:

```text
0.0001291081
```

### Final Approach

1. Strike-wise PCHIP interpolation
2. Iterative Imputer refinement

Public Score:

```text
0.0000731591
```

### Improvement

```text
0.0001291081 → 0.0000731591
```

Approximately 43% reduction in error.

## Repository Structure

```text
data/
notebooks/
results/
```

## Technologies

- Python
- Pandas
- NumPy
- SciPy
- Scikit-Learn

## Reproduction

Open:

```text
notebooks/Final_Submission.ipynb
```

Run all cells.

## Author

B Mithun
