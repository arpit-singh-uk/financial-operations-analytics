# Financial Operations Analytics: A Study in Synthetic Data for Banking Use Cases

> **Status:** Work in progress - currently building this end-to-end project and pushing each phase as it completes.

---

## Why this project

Synthetic data has been quietly maturing in UK financial services. The FCA set up its [Synthetic Data Expert Group](https://www.fca.org.uk/publications/corporate-documents/report-using-synthetic-data-financial-services) in March 2023, has since published two governance reports (the most recent in [August 2025](https://www.fca.org.uk/publications/corporate-documents/synthetic-data-models-financial-services-governance-considerations)), and built a dedicated synthetic dataset to support [Authorised Push Payment fraud detection](https://www.fca.org.uk/firms/digital-sandbox/authorised-push-payment-synthetic-data). In its [2026/27 annual work programme](https://www.fca.org.uk/news/news-stories/fca-sets-out-next-phase-smarter-more-effective-regulation), the FCA confirmed the Supercharged Sandbox will expand to give firms access to high-quality synthetic data for testing AI-driven financial products.

The reason this matters for analysts: real customer data in banking is largely locked behind GDPR, internal data governance, and regulatory scrutiny. It often cannot be used for exploratory work, model prototyping, or anything shared externally. Synthetic data is one of the practical workarounds the industry is actively investing in - the APP fraud dataset alone targets a category that cost UK consumers £485 million in 2022.

This project sits in that conversation.

---

## What this project does

An end-to-end financial analytics project covering three core problems any retail bank or subscription business cares about:

1. **Revenue forecasting** - predicting the next 12 months with usable accuracy, and what seasonality reveals about the business
2. **Customer churn** - who is likely to leave, why, and how much revenue is at risk
3. **Profitability and segmentation** - which customer segments actually drive profit, and where resources should be focused

The dataset is **AI-generated synthetic data designed to mimic real-world banking patterns**. That choice is deliberate, not a workaround. The project doubles as an informal stress test: **how close does AI-generated synthetic data actually get to behaving like the real thing?** The final phase will reflect on what the data captured well, where it broke down, and what that suggests about the role of synthetic data in real analytics workflows.

---

## Approach

The project tackles three problem areas. Specific techniques will be chosen during each phase based on what the data and business question require, with the reasoning documented in each phase commit.

| Problem area | What I will be looking at |
|--------------|---------------------------|
| Revenue forecasting | Time series patterns, seasonality, trend, forecast accuracy and uncertainty |
| Churn prediction | Identifying at-risk customers, understanding drivers, quantifying revenue at risk |
| Customer analytics | Segmentation, retention behaviour over time, customer lifetime value |

Techniques likely to feature across the project: time series methods (ARIMA family, Prophet, decomposition), classification models (logistic regression, tree-based ensembles), and unsupervised segmentation (RFM, clustering). Which techniques actually get used and why will be decided phase by phase.

**Tech stack:** Python, Pandas, NumPy, Scikit-learn, Statsmodels, Prophet, Matplotlib, Seaborn

---

## Project stages

**Phase 1** - Data generation and exploratory analysis  
**Phase 2** - Data preprocessing and feature engineering  
**Phase 3** - Revenue forecasting  
**Phase 4** - Churn modelling and risk stratification  
**Phase 5** - Profitability, RFM, and cohort analysis  
**Phase 6** - Executive dashboard and final reporting  
**Phase 7** - Reflection: how realistic was the synthetic data?  

Each phase will be committed as it completes, with notes on what worked, what did not, and what I would change.

## Further reading on synthetic data in UK financial services

- [FCA - Using Synthetic Data in Financial Services (2024 report)](https://www.fca.org.uk/publications/corporate-documents/report-using-synthetic-data-financial-services)
- [FCA - Generating and Using Synthetic Data: Governance Considerations (August 2025)](https://www.fca.org.uk/publications/corporate-documents/synthetic-data-models-financial-services-governance-considerations)
- [FCA - Authorised Push Payment fraud synthetic dataset](https://www.fca.org.uk/firms/digital-sandbox/authorised-push-payment-synthetic-data)
- [FCA - Annual work programme 2026/27](https://www.fca.org.uk/news/news-stories/fca-sets-out-next-phase-smarter-more-effective-regulation)