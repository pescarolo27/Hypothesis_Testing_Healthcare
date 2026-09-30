# Hypothesis Testing in Healthcare (Python)

**Background:** Pharmaceutical drugs have become an essential part of our health. Therefore, they need to be safe with little or no adverse effects.  
A pharmaceutical company, _GlobalXYZ_, has just completed a randomized controlled drug trial. To promote transparency and reproducibility of the drug's outcome, they (_GlobalXYZ_) have presented the dataset to your organization, a non-profit that focuses primarily on drug safety.

**The Data:** The dataset provided contained five adverse effects, demographic data, vital signs, & other medical information. Your organization is primarily interested in the drug's adverse reactions. It wants to know if the adverse reactions, if any, are of significant proportions. It has asked you to explore and answer some questions from the data. For this project, the dataset has been modified to reflect the presence and absence of adverse effects and the number of adverse effects in a single individual.

**Purpose:** You work with a non-profit that advocates for pharmaceutical drug safety. One of its tasks is to create reports on drugs independent of the drug manufacturer. 
Your organization has asked you to explore and answer some questions from the data collected. Conducting hypothesis tests using Python will help to determine if the adverse reactions of a hypothetical drug are significant or not. Other factors such as age will also be checked to see if they significantly influence the adverse reactions.  
The primary objectives are listed below.
1) Determine if the proportion of adverse effects differs significantly between the Drug and Placebo groups.
2) Find out if the number of adverse effects is independent of the treatment and control groups.
3) Examine if there is a significant difference between the ages of the Drug and Placebo groups.

This project was done in October, 2025.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Brief Summary
This project utilizes statistical techniques, primarily hypothesis tests, to evaluate some key objectives regarding individuals' health data & how it was impacted, if at all, by a new hypothetical drug that has been produced by _GlobalXYZ_.  
The control & treatment groups in the experiment conducted by _GlobalXYZ_ were analyzed in relation to whether individuals reported any adverse effects as well as how many they experienced. Other variables, such as peoples' ages, were also incorporated into the analyses.

A brief evaluation of the dataset revealed that two variables--the number of white & red blood cells--had missing values in more than 40% of the data points. Straightforward imputation methods were utilized to handle these problems, specifically the median & mean respectively.

To evaluate how the new drug affected individuals across the treatment & control groups, proportions of individuals in each were analyzed according to whether they experienced adverse effects or not. Note that of the 16,103 individuals, 10,727 of them were in the treatment (drug) group & 5,376 were in the control (placebo) group, which is about a 2:1 ratio.
- Initial analyses revealed that the percentage of individuals (within each control/treatment group) who did not experience adverse effects was about 90.45% & 90.48% in the treatment & control groups respectively.
- A two-sample proportion z-test was employed to further substantiate or oppose these findings. Ultimately, it produced a p-value of about 0.96 which is significantly greater than the typical significance level of five to ten percent. As such, this test indicated that there is no significant evidence from which the null hypothesis can be rejected. In other words, there is not a significant difference in the proportion of individuals who experienced adverse effects from the drug between the drug (treatment) & placebo (control) groups.

Next, to determine if the drug influenced the number of adverse effects that individuals experienced, the number of effects was analyzed across the treatment & control groups.
- Similarly to the first inquiry, initial analyses found that proportions of individuals across each number of adverse effects were very similar. For example, the percentage of people (within each treatment/control group) who experienced one adverse effect was approximately 8.91% & 9.04% for the treatment & control groups respectively.
- A chi-square hypothesis test was used to further investigate whether these two variables were independent or not. The smallest p-value obtained from the hypothesis test was about 0.50, which is much greater than a typical significance level of five to ten percent. As such, this test indicated that there is no significant evidence from which the null hypothesis can be rejected. In other words, the number of adverse effects experienced from using the drug is independent of whether an individual is in the control or treatment group.

Finally, the ages of the involved individuals were analyzed across the treatment/control groups to assess whether the drug impacted people differently according to their age.
- A brief analysis of ages across these two groups revealed quite similar averages & distributions. The average ages were about 64 years in each group.
- Given the nature of the data, a Mann-Whitney U test was used to further quantify this inquiry. The resulting p-value was about 0.26 which is noticeably larger than the pre-established significance level of five to ten percent. As such, this test failed to find substantial evidence with which to reject the null hypothesis. In other words, there is no significant difference between the ages of individuals in the treatment & control groups.


### Recommendations
These analyses reveal meaningful conclusions regarding some of the effects of the new drug produced by _GlobalXYZ_, specifically in regard to people experiencing adverse effects, the number of such effects, & people's ages. By evaluating these variables across control & treatment groups, it can be indicative as to the true effects of this drug.  
In all three sections of this project, it was determined that there is no significant relationship these three variables & the drug.
1) The proportion of individuals who experienced adverse effects from using the drug was not significantly different than that of those who did not use the drug.
2) The number of adverse effects experienced by individuals who used the drug was found to not be significantly different than the number of effects experienced by people who did not use the drug.
3) The ages of people across the control & treatment groups was not significantly different, therefore, generally ruling out age as a risk factor when using this drug.

As a result, these findings suggest that using the new drug does not pose any immediate concerns in terms of experiencing adverse effects. Furthermore, age is not a major concern, thus implying that the drug can be used by people of various ages. Additional analyses could be done to evaluate exactly how safe this drug is generally & for particular individuals according to different health qualities, demographics, & other specific details.
- Obviously, the nature of the drug should still be taken into account when it comes to who may be directed/allowed to take this drug. For instance, giving a new drug to young children is likely not a wise decision given that their bodies are still maturing.
