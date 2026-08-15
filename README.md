# SARIMA vs LSTM: Time-Series Forecasting of International Migration

A comparative time-series forecasting study evaluating a classical seasonal statistical model (SARIMA) against a recurrent neural network (LSTM) using monthly international migration estimates.

The objective is not to assume that deep learning is superior, but to evaluate both approaches under the same forecasting conditions and determine which model performs better on the held-out data.

---

## Research Question

> Can an LSTM neural network outperform a classical seasonal SARIMA model when forecasting monthly international migration estimates?

Both models are evaluated on the same final 12-month holdout period using Root Mean Squared Error (RMSE).

---

## Key Result

| Model | Test Horizon | RMSE |
|---|---:|---:|
| **SARIMA** | 12 months | **4.78** |
| **LSTM** | 12 months | **9.49** |

### Result

**SARIMA outperformed the LSTM model on the held-out 12-month period.**

The SARIMA model achieved an RMSE approximately **49.6% lower** than the LSTM.

This suggests that, for this dataset and forecasting configuration, the classical seasonal model captured the underlying temporal structure more effectively than the LSTM.

> **Important:** This result does not imply that SARIMA is generally superior to LSTM. It indicates that SARIMA performed better for this particular dataset, forecasting horizon, and model configuration.

---

## Dataset

The project uses monthly international migration estimates from the following dataset:

**International Migration - Citizenship by Visa and by Country of Last Permanent Residence**

The target variable used for forecasting is:

```text
estimate

