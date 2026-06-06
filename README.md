# Volatility Surface Reconstruction

## Objective

Reconstruct missing implied volatility values in a NIFTY options volatility surface.

---

## Dataset

- 975 timestamps
- 28 option contracts
- 5460 missing values
- Includes underlying price and implied volatilities

---

## Methods Evaluated

| Method | Score |
|----------|----------|
| Iterative Imputer | 0.0001291081 |
| PCHIP Interpolation | 0.0000731591 |
| Cubic Spline | 0.0002775212 |
| Akima Interpolation | 0.0014327977 |
| Moneyness PCHIP | 0.0000963289 |
| Linear Strike Interpolation | 0.0000423397 |

---

## Final Method

1. Separate call and put option chains
2. Sort contracts by strike
3. Apply linear interpolation across strikes
4. Generate reconstructed volatility surface
5. Create competition submission

---

## Best Public Leaderboard Score

0.0000423397
