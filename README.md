# Hypothesis Testing in Healthcare (Python)

**Background:** Pharmaceutical drugs have become an essential part of our health. Therefore, they need to be safe with little or no adverse effects.  
A pharmaceutical company, _GlobalXYZ_, has just completed a randomized controlled drug trial. To promote transparency and reproducibility of the drug's outcome, they (GlobalXYZ) have presented the dataset to your organization, a non-profit that focuses primarily on drug safety.

**The Data:** The dataset provided contained five adverse effects, demographic data, vital signs, etc. Your organization is primarily interested in the drug's adverse reactions. It wants to know if the adverse reactions, if any, are of significant proportions. It has asked you to explore and answer some questions from the data.

The dataset `drug_safety.csv` was obtained from [Hbiostat](https://hbiostat.org/data/) courtesy of the Vanderbilt University Department of Biostatistics. It contained five adverse effects: headache, abdominal pain, dyspepsia, upper respiratory infection, chronic obstructive airway disease (COAD), demographic data, vital signs, lab measures, etc. The ratio of drug observations to placebo observations is 2 to 1.

For this project, the dataset has been modified to reflect the presence and absence of adverse effects `adverse_effects` and the number of adverse effects in a single individual `num_effects`.

**The Purpose:** You work with a non-profit that advocates for pharmaceutical drug safety. One of its tasks is to create reports on drugs independent of the drug manufacturer.  
Your organization has asked you to explore and answer some questions from the data collected. You'll conduct several hypothesis tests using Python to determine if the adverse reactions of a hypothetical drug are significant. You'll also check if factors such as age significantly influence the adverse reactions.
1) Determine if the proportion of adverse effects differs significantly between the Drug and Placebo groups, saving the p-value as a variable called `two_sample_p_value`.
2) Find out if the number of adverse effects is independent of the treatment and control groups, saving as a variable called `num_effects_p_value` containing a p-value.
3) Examine if there is a significant difference between the ages of the Drug and Placebo groups, storing the p-value of your test in a variable called `age_group_effects_p_value`.

This project was done in October, 2025.
