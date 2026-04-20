###### fintech-transactions-risk-analysis



Exploratory data analysis and risk scoring of 6.3 million payment transactions

using the PaySim dataset. Built with Python, Pandas, NumPy, and Matplotlib.



\## Overview



This notebook analyzes a large synthetic mobile money transaction log to identify

fraud patterns and flag high-risk accounts. The analysis mirrors real-world fintech

data security workflows: aggregating transaction behavior, computing exposure scores,

and surfacing anomalies through visualization.



\## Dataset



\*\*PaySim1\*\* - Synthetic mobile money transactions generated to resemble real financial data.  

Source: \[Kaggle - PaySim1](https://www.kaggle.com/datasets/ealaxi/paysim1)  

Size: \~470MB, 6.3M transactions across 5 transaction types.



> Download the dataset from Kaggle and place it in the project root as `transactions.csv`.  

> The file is not included in this repo due to size.



\## Key Findings



\- Fraud occurs \*\*exclusively in TRANSFER and CASH\_OUT\*\* transactions - PAYMENT, DEBIT,

&#x20; and CASH\_IN show zero fraud activity across 6.3M records

\- Fraudulent transactions are heavily skewed toward \*\*high amounts\*\*, often draining

&#x20; accounts close to their full balance

\- A weighted risk scoring model successfully stratifies 6M+ accounts into

&#x20; \*\*Low / Medium / High\*\* risk tiers using fraud count, transaction volume,

&#x20; and single-transaction size

\- High-risk accounts represent a tiny fraction of users but concentrate

&#x20; disproportionate fraud exposure - consistent with real-world fraud concentration



\## Author



Sudarmathi Shenbagaraj  

\[github.com/sudarmathi2025](https://github.com/sudarmathi2025)



