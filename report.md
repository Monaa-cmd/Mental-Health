# Mental Health Report

## Descriptive analysis

1. The sample contains a group of participants whose age range from 18 to 60, with an average age of 39.
2. The sample is well-distributed and representative, with similar percentage of male and female samples, and the median value in each factors are also close to median value, except Work/Study hours, which has a distinctive higher standard deviation (3.77) compared to median (6).
3. There are a lot of missing values from the column 'Academic Pressure' , 'CPGA' and 'Study Satisfaction' (all around 80%) due to the fact that the survey is mainly aimed at working professionals. Therefore, this variable will not be taken into consideration for later analysis.
4. From the scatter plot, there are a few observation between several factors that potentially leads to depression.
    * Work/Study Hours vs. Depression
        Bottom-right scatter plots show that the orange points (Depression = Yes) are more common at higher work/study hours. This does suggest that longer work/study time might be associated with higher depression likelihood.

    * Job Satisfaction vs. Depression
        Orange points cluster toward lower job satisfaction values, indicating that lower satisfaction may be related to depression risk.

    * Work Pressure vs. Depression

        Orange points are more common in higher work pressure levels, though not as strong as the job satisfaction pattern. This fits with the idea that high work pressure could be a contributing factor.

    * Sleep Hours Numeric vs. Depression
        There’s no consistent linear pattern as both orange points in both low and high sleep durations. This could mean that sleep duration alone doesn’t explain depression risk — maybe sleep quality or sleep consistency would be more important, but those aren’t in the dataset.

    In conclusion, work pressure, job satisfaction, sleep duration, and work/study Hours are all correlated to some extent to potentially lead to depression. Therefore, the sample dataset serves a valid tool for our anlysis.

---

## EDA analysis
***Result***

A logistic regression was conducted to examine the factors associated with depression among 2,556 respondents. The model was statistically significant (LLR p < 0.001) and explained a substantial proportion of variance (Pseudo R² = 0.612).

---

Several predictors were found to have strong and significant associations with depression:


    * Suicidal thoughts emerged as the strongest predictor (OR ≈ 35.6, p < 0.001). Individuals who reported suicidal thoughts were more than 35 times as likely to report depression compared to those who did not.

    * Unhealthy dietary habits were also strongly associated with depression (OR ≈ 5.1, p < 0.001).

    * Work pressure increased the odds of depression nearly threefold (OR ≈ 2.7, p < 0.001).

    * Job satisfaction was protective: each unit increase in satisfaction reduced the odds of depression by approximately 63% (OR ≈ 0.37, p < 0.001).

    * Age was also protective (OR ≈ 0.74 per unit, p < 0.001), suggesting younger individuals had higher odds of depression.
---
With regard to sleep:

    * Sleeping more than 8 hours was associated with reduced depression risk (OR ≈ 0.55, p = 0.018).
    * Sleeping 7–8 hours showed a borderline protective effect (p = 0.052).

    * Sleeping less than 5 hours was associated with increased risk, though this was not statistically significant (p = 0.143).

    * Gender did not have a significant effect (p = 0.676).

***Discussion***

    The findings highlight the strong role of psychosocial and lifestyle factors in predicting depression. Consistent with previous literature, suicidal ideation was the most powerful predictor. Job-related stressors also played an important role: higher work pressure increased the risk of depression, whereas greater job satisfaction was protective.

    Dietary habits were another important predictor: unhealthy eating patterns significantly increased the odds of depression, supporting the growing body of evidence linking nutrition and mental health.

    Sleep duration showed mixed effects. While longer sleep (>8 hours) was protective, shorter sleep (<5 hours) increased risk but did not reach statistical significance. This may reflect sample size, measurement error, or the complexity of sleep–mental health interactions.

    Interestingly, gender was not a significant predictor in this sample, in contrast with some prior studies that report higher depression prevalence among females. This suggests that other lifestyle and psychosocial factors may play a more dominant role in this dataset.

to do:
fix draft for descriptive analysis
details in EDA report(question, etc.): protective?
solution (action fro HR)