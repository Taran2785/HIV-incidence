HIV Incidence in Canada: A Data-Driven Approach Using Difference-in-Differences (DiD)

Overview

This project analyzes HIV incidence trends in Canada from 2000 to 2024, focusing on the impact of Pre-Exposure Prophylaxis (PrEP) introduction using the Difference-in-Differences (DiD) methodology. The analysis evaluates HIV incidence rates across three age groups:

 Data source: World Bank Data

All Ages

Ages 15-49

Ages 15-24

By leveraging statistical techniques, we aim to assess how public health interventions like PrEP have influenced HIV incidence over time.

Data Sources

The dataset used in this project includes:

HIV Incidence Rates (per 1,000 uninfected population)

PrEP Introduction Indicator (binary variable: 0 = pre-PrEP, 1 = post-PrEP)

Country and Year Variables

The data was sourced from publicly available datasets on Our World in Data and other relevant public health sources.

Methodology

Difference-in-Differences (DiD) Model

The DiD methodology compares HIV incidence trends before and after PrEP introduction, isolating the effect of PrEP by accounting for time-varying factors.

The model specification:

HIV Incidence = β₀ + β₁ (Post_PrEP) + β₂ (Treatment) + β₃ (DiD_Term) + γ (Country) + δ (Year) + ϵ

Where:

β₁: Effect of PrEP introduction on HIV incidence

β₂: Treatment effect (Canada)

β₃: Interaction term (DiD estimator, capturing the causal effect of PrEP)

γ, δ: Country and year fixed effects

Results & Key Findings

Significant Decline in HIV Incidence: The introduction of PrEP led to a notable reduction in HIV incidence, particularly in the 15-49 and 15-24 age groups.

Statistical Significance: The interaction term (DiD_Term) was statistically significant, suggesting a causal relationship between PrEP introduction and declining HIV incidence.

Confidence Interval Variability: The confidence interval widened around 2020, potentially due to COVID-19 disruptions affecting HIV testing and reporting.

Visualization

Several visualizations were generated to illustrate the findings:

Line Graphs: Showing pre- and post-PrEP trends in HIV incidence.

Bar Charts: Comparing HIV incidence across different age groups.

DiD Plots: Highlighting the impact of PrEP introduction.

Example code to generate and save visualizations:

Installation & Setup

To run this project locally, follow these steps:

Clone the Repository

Install Dependencies

pip install -r requirements.txt

Run the Analysis

python analysis.py

Future Work

Apply similar DiD models to other countries for a global comparison.

Integrate additional variables like healthcare access, education, and sexual behavior trends.

Use machine learning for predictive modeling of future HIV incidence trends.

