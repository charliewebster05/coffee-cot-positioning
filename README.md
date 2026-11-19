# coffee-cot-positioning
Does fund positioning in coffee futures predict returns? CFTC COT data, 2006–2026.

# Fund positioning in coffee futures (2006–2026)

Tests whether managed-money positioning in ICE Coffee C predicts returns over the following 4 and 12 weeks.

**Data:** CFTC Commitments of Traders (disaggregated) and KC=F prices from yfinance.

**Method:** rolling 3-year z-score of net positioning, returns from the Monday after each Friday release,
OLS with Newey-West errors, an out-of-sample split and an episode-level sign test.

**Findings**
- No overall linear relationship
- Very long positioning was followed by 4-week returns 3.9 points lower than other weeks (p = 0.009)
- Consistent in direction across both halves of the sample, but stronger after 2016
- 9 of 12 crowded-long episodes were followed by losses

**Caveats:** only 12 independent episodes, threshold chosen after looking at the data, no trading costs.

**Files:** `Crowded Longs in Coffee - Does Fund Positioning Predict Returns?.ipynb` (code), `Crowded Longs in Coffee- Does Fund Positioning Predict Returns?.pdf` (write-up)
