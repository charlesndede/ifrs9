# ✍🏻 IFRS 9 Impairment model 
![Google Colab](https://img.shields.io/badge/Editor-Google%20Colab-brightgreen)
![Python](https://img.shields.io/badge/Code-Python-blue)

<p align="center">
  <img src="https://user-images.githubusercontent.com/66057952/194217235-5c62f839-1390-44a7-b71d-82a29c53805e.png" alt="ifrs 9"/>
</p>

The IFRS 9 requires recognition of impairment losses on a forward-looking basis, which means that impairment loss is recognised before the occurrence of any credit event. These impairment losses are referred to as Expected Credit Losses **('ECL')**.

## The general approach
The general IFRS 9 Approach to impairment follows a three stages model _(sometimes referred to three-bucket model)_:

<p align="center">
  <img src="https://github.com/naenumtou/ifrs9/assets/66057952/97a52b90-ea60-4067-bb3d-7c9c389f3160" alt="ifrs 9 three-buckets model"/>
</p>

As it can be seen that under the general approach, an entity recognises expected credit losses for all financial assets. The ECL can be 12-month ECL or lifetime ECL depending on whether there was a significant increase in credit risk _(IFRS 9.5.5.3)_.
1. **12-month ECLs (Stage 1)**: It is applied to all the loans since initial recognition as long as there is low credit risk
2. **Lifetime ECLs (Stages 2 and 3)**: It is applied when a significant increase in credit risk has taken place

## The measurement of expected credit losses (ECL)
### Definition of credit losses
Credit loss is the difference between all contractual cash flows that are due to an entity in accordance with the contract and all the cash flows that the entity expects to receive, discounted at the original Effective Interest Rate (EIR) or credit-adjusted EIR _(IFRS 9 Appendix A)_.

### Model components
* **PD** is a probability of default model to estimate potential loss that likely to occur in given time period.
* **LGD** is a loss given default to calculate occured loss that the loan cannot be paid.
* **EAD** is a exposure at default to calculate outstanding balance of the loan having in default stage.

The model components will be appiled together with **staging criteria**, which is allowed ECL Calculation of different risk segmentation. This is to be more accuracy for the Bank's provisioning processes.

### The calculation workflow

<p align="center">
  <img src="https://www.moodysanalytics.com/-/media/web-assets/publications/risk-perspectives/edition-images/v-data-management/articles/2-4-ifrs-9-expected-loss-impairment-model/fig-2-ifrs-9-workflow.png?modified=20150515184530" alt="ifrs 9 calculation workflow"/>
</p>

From this data, the Bank can implement models on PD, LGD, and EAD, combining external data such as macroeconomic forecasts to get 12-month and lifetime expected loss forecasts _(discounted at current interest rates or EIR)_. Then, based on exposure and counterparty characteristics, allocation between stages 1, 2, and 3 sends the final EL provision to accounting systems.
