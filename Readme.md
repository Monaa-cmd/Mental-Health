# Mental Health Project

This project explores factors related to mental health using Python. It will analyze how factors like gender, age, family history, and remote work affect mental health in tech. Potentially machine learning would also be applied to particularly investigate the major factors that contribute to mental well-being.

# About Dataset
[web page link] https://www.kaggle.com/datasets/sumansharmadataworld/depression-surveydataset-for-analysis

This dataset was collected as part of a comprehensive survey aimed at understanding the factors contributing to depression risk among adults. It was collected during an anonymous survey conducted between January and June 2023. The survey was conducted across various cities, targeting individuals from diverse backgrounds and professions. Participants, ranging from 18 to 60 years old, voluntarily provided inputs on factors such as age, gender, city, degree, job satisfaction, study satisfaction, study/work hours, and family history among others. Participants were asked to provide inputs without requiring any professional mental health assessments or diagnostic test scores.

## Features
- Uses virtual environment
- Data analysis with pandas, seaborn
- Visualizations with matplotlib
- Machine Learning

## Getting Started
To activate the environment:

```bash
.venv\Scripts\Activate.ps1
```

- Ask:  
    [Descriptive analysis]
    correlation (scatterplots matrics to see relation)

    [EDA]
    
    What factors lead to higher tendency towards depression? And the major factors? [logistic regression]

    Does job satisfaction/dietary habits lead to higher chances of depression? [T-test/ANNOVA between depressed and group with normal well-being] 

    [Solutions concerning HR: What can HR do to improve the well-being of employees?]
    Should remote or hybrid work be promoted?
    Promotion of healthy lifestyle [sleep and eating]
    Explore trends in seeking help and employer support.
    Potential things to consider [exercise, compensation, package and bonus to support individuals under higher pressure]

    [ML]

- Prepare
- Process
- Analyze
    Pitfall
- Share
- Act




[Descriptive analysis]
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

    In conclusion, work pressure, job satisfaction, sleep duration, and work or study Hours are all correlated to some extent to potentially lead to depression. Therefore, the sample dataset serves a valid tool for our anlysis.


[EDA]
logistic regression test [continue]
work/study hours ANNOVA test
