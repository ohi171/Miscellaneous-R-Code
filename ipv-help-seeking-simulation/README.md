# Healthcare contact, partner control, and help-seeking

This exercise prepares a reproducible analysis for a proposed secondary-data study: **among ever-married women aged 18–49 reporting past-year physical or sexual partner violence, does the association between recent healthcare contact and formal violence-related help-seeking differ by reported partner controlling behaviours?**

The motivation is to examine whether a healthcare encounter has the same association with formal help-seeking across different relationship circumstances. Simulating the study first helps clarify the variables, interaction model, and interpretation before analysing survey data.

The [R script](simulated_ipv_analysis.R) generates 10,000 fictional observations and fits a logistic regression with a healthcare-contact × partner-control interaction, adjusting for violence severity, sexual violence, age, education, wealth, and urban residence. The central result is the difference between the two adjusted contact associations, expressed in percentage points with 95% confidence intervals. This probability-scale comparison complements the odds-scale interaction.

## Run

Open `simulated_ipv_analysis.R` in RStudio and click **Source**. Only base R is required. The script creates `SIMULATED_IPV_analysis` in the current working directory, containing the dataset, variable dictionary, results tables, figure, and a simulated results paragraph. Re-running replaces these generated outputs.

**All data and results are fictional.** The hypothesized interaction is deliberately built into the simulation. This is an analysis-development exercise, not empirical evidence or a power analysis. The code has not been runtime-tested in the authoring session.

The example assumes three-month healthcare contact and past-year help-seeking; it cannot establish temporal ordering or causality. An actual NFHS application requires verified variable definitions, recall periods, survey weights, strata, and clusters.
