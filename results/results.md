## 1.1 Portfolio overview
How big is the loan portfolio?

| total_loans | total_exposure | avg_loan | smallest_loan | largest_loan | avg_duration_months |
|---|---|---|---|---|---|
| 350 | 1,167,451 | 3,336 | 276 | 15,945 | 20.9 |

**Finding:** The portfolio has 350 loans worth about 1.17 million in total. The average loan is about 3,336 and lasts about 21 months. The largest loan (15,945) is almost five times the average, so a few large loans may carry a lot of the risk.
SELECT SUM(saving_accounts  IS NULL) AS missing_savings,
       SUM(checking_account IS NULL) AS missing_checking,
       SUM(saving_accounts IS NULL AND checking_account IS NULL) AS missing_both
FROM loans;
