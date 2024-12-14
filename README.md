# Data Analysis Portfolio

This repository showcases three distinct data analysis projects, showcasing my skills in exploratory data analysis, model selection, and designing simulation studies. 

## Project 1
### Exploratory Data Analysis on the Relationship Between Environmental Conditions and Marathon Performance

**Background**:  This project is a collaboration with Dr. Brett Romano Ely and Dr. Matthew Ely from the Department of Health Sciences at Providence College. The report explores the relationship between environmental conditions and marathon performance. There's well documented sex difference between marathon performance and their response to environmental conditions. Age difference in marathon performance and their response to environmental conditions is also shown in previous studies. The data used in this analysis was collected from the 5 major marathons (Boston, Chicago, NYC, Twin Cities, and Grandma's).

**Methods**: This report explores the relationship between environmental conditions and marathon performance. The goal is to investigate (1) the effects of increasing age on marathon performance in men and women, (2) the impact of environmental conditions on marathon performance, and whether the impact differs across age and gender, and (3) which weather parameters (WBGT, Flag conditions, temperature, etc) that have the largest impact on marathon performance. The data used in this analysis was collected from the 5 major marathons (Boston, Chicago, NYC, Twin Cities, and Grandma's) from years 1993 and 2016 for a total of 11564 race records. The full report can be found [here](Exploratory Data Analysis/Report files/marathon EDA analysis.pdf). 

**Results**: The analysis reveals the influence of environmental conditions, particularly black globe temperature, dry bulb temperature, wet bulb temperature, and dew point, on marathon performance. The relationship between WBGT and performance follows a U-shaped curve. Women experience a more accelerated decline in marathon performance as they age compared to men, especially in the 55-64 and 65+ age groups. The analysis also shows older age groups are more sensitive to heat and humidity, and therefore the impact of environmental conditions on marathon performance differs across age groups. Full report can be found [here](<Exploratory Data Analysis/Report files/marathon EDA analysis.pdf>).

## Project 2
### Moderation Analysis and Prediction of Smoking Abstinence in Behavioral Therapy and Pharmacotherapy

**Background**: Previous randomized, placebo-controlled 2x2 factorial design in smokers with major depressive disorder (MDD) comparing behavioral activation for smoking cessation (BASC) versus standard behavioral treatment (ST) and varenicline versus placebo has discovered varenicline improved smoking abstinence. This is a follow-up analysis for the study to examine baseline variables as potential moderators of the effects of behaviorial treatment on abstinence and evaluate baseline variable as predictors of abstinence, controlling for behavioral treatment and pharmacotherapy.

**Methods**: We used LASSO regression and Best Subset regression with $L_0+L_2$ regularization to perform moderation analysis to investigate the factors influencing smoke cessation and efficacy of the treatment. Multiple imputation was used to address missing data. In addition, models were evaluated using area under the receiver operating characteristic curve (AUC), Brier score, calibration plot, accuracy, sensitivity, and specificity.

**Results**: Predictors of smoking cessation and treatment moderators were identified; Morning smoking habits and nicotne metabolism were two pronouced moderators identified for varenicline. Baseline characteristics such as non-hispanic white, income, and FTCD score are selected as significant predictors of smoking abstinence. However, there are some uncertainty regarding the significance of the coefficients. Larger and more diverse samples are needed to validate these findings and enhance their reliability. Full report can be found [here](<Regression and Moderation Analysis/Report files/Regression and moderation analysis.pdf>).

## Project 3
### Determine the optimal study design under a fixed budget using simulation

**Background**: This project explores the impact of study design parameters on the precision of treatment effect estimates $\hat{\beta}$ in cluster-randomized trials under a fixed budget constraint. We aim to determine the optimal study design that lowers the variance of the treatment effect estimates. 

**Model Framework**:
For $Y_{ij} \sim$ normal distribution:

- Cluster-level mean: $\mu_i \mid X_i, \epsilon_i = \alpha + \beta X_i + \epsilon_i, \text{where} \epsilon \sim N(0, \gamma^2)$ We generate the cluster-level mean from a normal distribution with mean $\mu_{i0} = \alpha + \beta X_i$ and variance $\gamma^2$.

- Subject-level outcome: $Y_{ij} \mid \mu_i, e_{ij} = \mu_i + e_{ij}, \quad e_{ij} \sim N(0, \sigma^2)$ We generate the - subject-level outcome from a normal distribution with mean $\mu_i$ and variance $\sigma^2$.

For $Y_{ij} \sim$ Poisson distribution:

- Group-level mean: $\log(u_i) \sim N(\alpha + \beta X_i, \gamma^2)$ We generate the cluster-level mean from a normal distribution with mean $\mu_{i0} = \alpha + \beta X_i$ and variance $\gamma^2$, and exponentiate it to get the mean counts $\mu_i$

- Subject-level outcome: $Y_{ij} \mid \mu_i \sim Poisson(\mu_i)$ for each subject in the cluster We generate the subject-level outcome from a Poisson distribution with mean $\mu_i$.

**Methods**: A simulation-based approach was used to assess the estimator's performance across various parameter configurations. The data were modeled using hierarchical structures with binary treatment assignments. Under the normal distribution framework, the variance of the outcome and the sampling error were treated as independent contributors, whereas the Poisson distribution assumed that the mean and variance were equal. The impact of differing budget levels, cost ratios, and parameter values on the estimator’s standard error was evaluated. A grid search methodology was utilized to determine the optimal trade-off between the number of clusters and the number of measurements within each cluster.

**Results**: The optimal study design is determined by minimizing the variance of the treatment effect estimates Var($\hat{\beta}$). The optimal study design is largely influenced by the between cluster correlation $\gamma$, and the budget constraint's relative cost ratio $c_1/c_2$. More details can be found in the [report](<Simulation Study/Budget constraint simulation.pdf>)

## Contact Information
**Miaoyan Chen** \
Miaoyan_chen@brown.edu \
[LinkedIn](https://www.linkedin.com/in/miaoyanchen/) \
[Github](https://github.com/miaoyanchen)
