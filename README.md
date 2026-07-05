# JPMorgan Chase Quantitative Research Job Simulation

Completed as part of the Forage JPMorgan Chase Quantitative Research virtual job simulation.
Covers natural gas price forecasting, commodity storage contract pricing, and credit risk modeling.

## Task 1 & 2: Natural Gas Pricing & Storage Contract Valuation
File: `Task1_2_Gas_Pricing.ipynb`

- **Task 1:** Built a price estimation model using historical monthly natural gas prices (Oct 2020 - Sept 2024). Combined a linear trend with a seasonal (sinusoidal) component to interpolate historical prices and extrapolate up to 1 year into the future.
- **Task 2:** Built a `price_contract()` function to value gas storage contracts, generalized to support multiple injection/withdrawal dates. Accounts for purchase/sale cash flows, storage costs, injection/withdrawal fees, and volume/rate constraints.

**Key techniques:** Linear regression, time series feature engineering, cash flow modeling.

## Task 3 & 4: Loan Default Risk Modeling
File: `Task3_4_Loan_Default_Model.ipynb`

- **Task 3:** Built a probability-of-default (PD) model on a personal loan dataset (10,000 borrowers) using logistic regression, with a decision tree built as a comparison model. Produced a `predict_expected_loss()` function combining PD with a 10% recovery rate assumption.
- **Task 4:** Built a FICO score quantization tool using dynamic programming to bucket scores into rating categories, optimizing for log-likelihood of observed defaults. Produces a general `rating_map()` function where a lower rating indicates better credit quality.

**Key techniques:** Logistic regression, decision trees, dynamic programming, log-likelihood optimization.

## Tools
Python, pandas, numpy, scikit-learn, matplotlib, Google Colab
