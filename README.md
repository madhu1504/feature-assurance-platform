# feature-assurance-platform
Data science project evaluating user engagement across countries with hierarchical modelling and simulation-based power analysis.
# Evaluating the Impact of a Milestones Feature on User Engagement

## Project Overview

This project evaluates the effectiveness of a newly introduced **"Milestones"** feature for *InstaGrammar*, a fictional language learning platform. The feature was rolled out to approximately half of users across 12 countries, creating a large-scale natural experiment to measure its effect on weekly app engagement.

The analysis uses **Linear Mixed-Effects Models (LMMs)** to account for the hierarchical structure of users nested within countries and compares a **Random Intercept Model** with a **Random Intercept + Random Slope Model** to determine whether feature performance varies geographically.

A stochastic simulation-based power analysis** is then conducted to estimate the minimum sample size required for a future **"Daily Streaks"** experiment while achieving **90% statistical power**.

## Key Objectives

* Evaluate whether the **Milestones** feature significantly increases weekly app engagement.
* Compare alternative mixed-effects model specifications using likelihood ratio testing.
* Quantify country-level variation in baseline engagement and feature effectiveness.
* Estimate the minimum sample size required for future A/B testing using stochastic simulation.
* Provide evidence-based product recommendations for feature rollout strategy.

## Methods

* Linear Mixed-Effects Modelling (`lme4`)
* Random Intercept and Random Slope Models
* Intraclass Correlation Coefficient (ICC)
* Likelihood Ratio Test (LRT)
* Model Diagnostics and Assumption Checking
* Monte Carlo Simulation
* Statistical Power Analysis
* Data Visualisation with `ggplot2`

## Key Findings

* The **Milestones** feature increased average weekly engagement by approximately **11 minutes per user**.
* A **Random Intercept + Random Slope Model** provided a substantially better fit than a Random Intercept Model, demonstrating that feature effectiveness differed across countries.
* Around **58% of engagement variability** was attributable to country-level differences when heterogeneous feature effects were modelled.
* Simulation-based power analysis indicated that **approximately 1,000 participants** would be required to achieve **90% statistical power** for a future experiment with a similar expected effect size.

## Skills Demonstrated

* Mixed-effects regression modelling
* Hierarchical data analysis
* Experimental design and A/B testing
* Statistical inference
* Monte Carlo simulation
* Power analysis
* Data visualisation
* R programming (`tidyverse`, `lme4`, `ggplot2`, `lmerTest`, `performance`)

## Repository Structure

* `analysis.Rmd` – Complete statistical analysis and report
* `opt1_app.csv` – Dataset
* `figures/` – Generated visualisations
* `README.md` – Project overview and summary
