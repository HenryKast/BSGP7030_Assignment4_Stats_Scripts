# Prompts

## Prompt 1

Begin with a blank slate, do not use any other repositories or past conversations to guide you. I have created a folder for you to work in, it is bash_tutorial/assignment_4/Ai.	I would like you to begin in a notebook titled stats_python. The general overview of this project will be Data representation and interaction
Data as a table
The pandas data-frame
Hypothesis testing: comparing two groups
Student’s t-test: the simplest statistical test
Paired tests: repeated measurements on the same individuals
Linear models, multiple factors, and analysis of variance
“formulas” to specify statistical models in Python
Multiple Regression: including multiple factors
Post-hoc hypothesis testing: analysis of variance (ANOVA)
More visualization: seaborn for statistical exploration
Pairplot: scatter matrices
lmplot: plotting a univariate regression.			Begin with the data representation and interaction using the brain_size.csv for data. Within this section I would like to create general dataframes, grouby_gender dataframes, mean VIQ for full population, total number of males/females. I would like the data plotted in scatter matrices. I would like combined matrices, male only, and female only matrices. After this is completed we will move on to statistical analysis

## Prompt 2

Continue with statistical analysis. I want to include tests if FISQ and PIQ are signifigantly different, male vs female tests if mean VIQ is different, the difference between weights in males and females, and non parametric stats to test the difference between VIQ in males and females

## Prompt 3

Continue with linear models and analysis of variance. Begin with the brain_size.csv . Create a dataframe with the data. Specify an OLS model and retreive the parameters from the model used. After this, compare different types as well as a general IQ between males and females. Next, using iris.csv create a dataframe with the goal of answering "Sepal and petal size tend to be related: bigger flowers are bigger! But is there in addition a systematic effect of species?". Run an F test if there is any difference between versicolor and virginica after removing the effect of sepal width. After this go back the the brain_size.csv and test if the VIQ of males and females are different after removing the effect of brain size, height, and weight.

## Prompt 4

Next we will use seaborn with the wages.txt file to display scatter matrices and plot a univariate regression between wage and education
