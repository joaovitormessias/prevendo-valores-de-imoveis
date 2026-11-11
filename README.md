# House Price Regression

**Compare interpretable linear models and inspect the limits of house-price prediction.**

This educational notebook explores property attributes, fits ordinary least-squares models, examines multicollinearity and residuals, and predicts prices for a bundled set of new houses. It is not a property appraisal service.

## Reproduced result

| Final model measurement | Value |
| --- | --- |
| Training R² | 0.6511 |
| Held-out test R² | 0.6432 |
| Test split | 30%, random_state=230 |

Values were reproduced during review using the notebook's existing split and model. R² is not percentage prediction accuracy. Model selection is exploratory; there is no untouched external validation set or deployed prediction API.

## Model inputs

The final model uses first-floor area, the presence of a second floor, bathroom count, and an excellent-kitchen indicator, plus an intercept. The notebook compares this with larger specifications and computes variance inflation factors.

## Run locally

```bash
git clone https://github.com/joaovitormessias/prevendo-valores-de-imoveis.git
cd prevendo-valores-de-imoveis
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook prevendoValoresDeImoveis.ipynb
```

If Jupyter is not available in your environment, install it with `pip install jupyter`. Run from the repository directory so the relative `dataset/` paths resolve.

## Review the analysis

- [Notebook](prevendoValoresDeImoveis.ipynb): EDA, train/test split, OLS comparisons, predictions, VIF, and residual plots.
- [Training data](dataset/Preços_de_casas.csv): bundled input data.
- [New houses](dataset/Novas_casas.csv): illustrative prediction inputs.

The single-house prediction now passes a DataFrame to the formula-based model, preserving named-column lookup. The test-R² comment is corrected to distinguish held-out evaluation from training fit.

## Verification and limitations

All 58 nonempty code cells executed sequentially during review, with chart display suppressed. Interactive plots were not visually checked. Dataset provenance, units, representativeness, and collection methodology need better source documentation before interpreting prices operationally.

Coefficients are associations, not causal effects. Add a naive baseline, MAE/RMSE, cross-validation, and prediction-interval assessment before comparing practical usefulness. Residual and collinearity diagnostics do not establish production reliability.

[MIT license](LICENSE) · [Maintainer](https://github.com/joaovitormessias)
