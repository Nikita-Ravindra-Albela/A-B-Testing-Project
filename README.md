## A-B-Testing-Project
This project demonstrates how to design, execute, and analyze an A/B test using a statistically sound framework. A real-world scenario was simulated: does a new website design improve conversions?

## Project Overview

Synthetic dataset of 2,000 website visitors

Group A = Control (old design)

Group B = Variant (new design)

Conversion rate is the KPI

Two-Proportion Z-Test used for statistical significance

## Technologies Used

Python (Pandas, NumPy)

Statsmodels

A/B Testing Statistics

Hypothesis Testing

## Dataset Description

Each visitor record contains:

Column	Meaning
group	A or B
converted	0 or 1

A represents old design.
B represents new design.

## Conversion Rates
Group	Conversion Rate
A	10%
B	14%

## Statistical Test

Test: Two-Proportion Z-Test

Test Implementation
from statsmodels.stats.proportion import proportions_ztest

z_stat, p_value = proportions_ztest(successes, samples)

Result

Z = -2.94

p = 0.0032

✔ Interpretation

p < 0.05 → statistically significant

New design improves conversions

+4% absolute uplift

+40 conversions per 1,000 visitors

## Business Impact

If the site gets 1M visitors/month, expected impact:

40,000 additional monthly conversions

Major uplift in revenue and customer engagement

## Skills Demonstrated

Experiment design

Hypothesis testing

Statistical analysis

Python data analysis

Communicating business impact
