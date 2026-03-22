# Silver Fund Bayesian Reversal Repository

## Set Up

Set up your Python virtual environment using `uv`.
```bash
uv sync
```

Source your Python virtual environment.
```bash
source .venv/bin/activate
```

Set up your environment variables in a `.env` file. You can follow the example found in `.env.example`.
```
ASSETS_TABLE=
EXPOSURES_TABLE=
COVARIANCES_TABLE=
CRSP_DAILY_TABLE=
CRSP_MONTHLY_TABLE=
CRSP_EVENTS_TABLE=
BYU_EMAIL=
PROJECT_ROOT=
```

Set up pre-commit by running:
```bash
prek install
```

Now all of your files will be formatted on commit (you will need to re-commit after the formatting).

## Experiments
1. Baseline BMA Reversal (3-Horizons)
2. Dynamic Weighting and Recency Decay
3. Hierarchical Bayesian Update (Prior vs. Likelihood)
4. Bayesian Shrinkage via the Null Model
5. Information Filtering (Volume Inhibition)
6. Winsorized Volume-Inhibited BMA
7. Alpha Smoothing (EWMA Decay)
8. Signal Acceleration & Risk Scaling
9. Correlation and Bivariate Regression Test (BMA Rev. vs Enhanced Rev.)
10. Sample Portfolio Active Risk & Attribution