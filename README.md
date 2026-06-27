# Securitisation Risk Arena & Credit Dashboard

An end-to-end data analytics framework designed to assess credit risk, calculate regulatory impairments, and simulate structural payment waterfalls for structured credit asset pools.

##  Tech Stack & Architecture
* **Data Source:** Simulated core banking SAP/ERP auto-loan subledgers.
* **Risk Modeling:** Python (pandas, numpy) for macro-stress simulations and IFRS 9 Stage allocations.
* **BI Architecture:** Microsoft Power BI / SSAS utilizing a Star Schema data model and advanced DAX engine.

##  Core Features Implemented
1. **Star Schema Data Model:** Linked master `Dim_Calendar` with transactional tables via 1:Many relationships.
2. **IFRS 9 ECL Engine:** Built measures calculating Expected Credit Losses ($EAD \times PD \times LGD$).
3. **Macroeconomic Stress Testing:** Created dynamic DAX simulations evaluating portfolio impairment shifts under severe financial downturns.
4. **Structured Asset Waterfall:** Modeled sequential-pay mechanisms distributing cash flows down Senior and Subordinated tranches.

##  Dashboard Preview
* **Time-Series Slicer:** Filters historical eras from the 2024 closing horizons.
* **Pool Amortization Gauge:** Tracks asset contraction boundaries relative to required safety liquidity levels.
