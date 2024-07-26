## Cure model in survival analysis 

A cure model is a type of survival analysis model that accounts for the possibility that a proportion of the study population is "cured" and will not experience the event of interest (e.g., death, recurrence of disease). This approach is particularly useful in medical research, where treatments can result in long-term remission or cure for some patients.


### Purpose of Cure Models
The primary purpose of cure models is to provide a more accurate analysis of survival data in scenarios where a substantial proportion of individuals are expected to be cured. Cure models separate the population into two subgroups:

#### Cured Group: 
Individuals who are cured and will not experience the event of interest.
#### 
Uncured Group: Individuals who are not cured and remain at risk of the event.

### Key Concepts

#### Cure Fraction: 
The proportion of the population that is considered cured.
#### Incidence: 
The probability of an individual being in the cured group versus the uncured group.
#### Latency: 
The time to the event of interest for those who are not cured.

### Types of Cure Models

#### Mixture Cure Models:

Assumes that the population is a mixture of cured and uncured individuals.

Models the survival function as a combination of a cure fraction and the survival function for the uncured.

### Non-mixture Cure Models:

Models the hazard function such that it eventually converges to zero, reflecting that some individuals are cured.


## cuRe Package
#### Purpose
Designed specifically for fitting cure models in survival analysis.
#### Key Features
##### Cure Models: 
Supports both mixture and non-mixture cure models.
##### Baseline Hazards: 
Allows for various parametric distributions for baseline hazards, such as Weibull, log-normal, and log-logistic.
##### Covariate Inclusion: 
Permits the inclusion of covariates in both the incidence (cure fraction) and latency (time to event) parts of the model.
##### Goodness-of-fit: 
Provides diagnostic tools and goodness-of-fit measures for model evaluation.
#### Typical Use Cases
Medical studies where a portion of patients are expected to be cured.
Long-term follow-up studies with the potential for a cure.

## flexsurvcure Package
#### Purpose
Part of the flexsurv package, designed for flexible parametric modeling of survival data, including cure models.
#### Key Features
##### Flexible Parametric Models: 
Supports a wide range of parametric distributions (exponential, Weibull, gamma, log-normal, log-logistic, etc.).
##### Custom Distributions:
Allows users to define custom survival distributions.
##### Cure Models:
Supports both mixture and non-mixture cure models within the flexible framework.
##### Multi-state Models: 
Provides tools for modeling multi-state processes.
#### Typical Use Cases
General survival analysis with the need for flexibility in choosing or defining distributions.
Situations where a combination of parametric models and cure models is required.


## rstpm2 Package
#### Purpose
Provides flexible parametric modeling of survival data using spline-based approaches.
#### Key Features
##### Spline-based Models: 
Uses splines to model the baseline hazard function flexibly.
##### Time-varying Effects: 
Supports modeling of time-varying covariate effects.
##### Multi-state Models: 
Capable of fitting multi-state models.
##### Diagnostics and Plots: 
Includes various diagnostic tools and plotting functions for model evaluation.
#### Typical Use Cases
Complex survival data requiring flexible modeling of hazard functions.
Analysis where time-varying covariate effects are important.
Scenarios involving multi-state processes.

[Jupyter notebook for a work-out example](https://github.com/BhadraNivedita/Cure-model-in-Survival-analysis) 




