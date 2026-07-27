# Overview
This repository aimed to explore statstical analysis using python. Using multiple datasets, and multple modeling methods
it follows my process of learning following the SciPy tutorial

## Repository Structure
There are two distinct folders in this repo.
Ai/                # AI-assisted notebook
  stats_python.ipynb
  brain_size.csv
  iris.csv
  wages.txt
  prompts.md

Manual/            # Manual notebook
  BSGP7030_Assignment4_Stats_Scripts/
    Notebooks/
    environment-4.yml
    .gitignore

## Datasets
brain_size.csv      Contains Gender, FSIQ, VIQ, PIQ, Weight, Height, and MRI_Count measurments
iris.csv            Contains iris sepal and petal measuremnets by species
wages.txt           Contains wage data including education, experience, wage, and demographic

## Analysis Outline
Data representation - pandas DataFrames, groupby, summaries, scatter matrices
Hypothesis testing - paired/unpaired t-tests
Linear models & ANOVA - IQ comparisons, iris species F-tests, adjusted VIQ F-test
Seaborn visualization - pairplotm, lmplot
Bayesian alternatives (Ai only) - PyMC/bambi for key comparisons

## Environment / Setup
Conda environment utilizing pandas, scipy, statsmodels, and seaborn

### Creating and activating the environment
conda env create -f environment-4.yml
conda activate 7030_class_4
### Running the notebooks
cd Notebooks  # Manual notebook
#Cd /Ai       # Ai Notebook
jupyter lab
### AI notebook extras
The base environment does not cover pymc, arviz, bambi used by the Ai version
conda activate 7030_class_4
pip install pymc arviz bambi

## How to run
Run all cells should run with no issues with all dependencies installed in the environment.


## Manual vs AI
### Where they agree
Both versions have many brain-size conclusions matches, mean VIQ between males and females is insignifigant (p=0.445), 
weight is signifigant (p-2.2e-5) Mann-Whitney of VIQ is insignifigant, paired FSIQ-PIQ is insignifigant (p=0.082). 
VIQ ~ Gender and adjusted VIQ agree.

### Where they differ
FSIQ vs PIQ - Manual runs an unpaired + paired, + wilcoxon, AI runs paired only
IQ OLS - AI ran many more comparison between the different types of IQ than manual

Wages - Manual uses log10(WAGE) + EDUCATION*SEX, AI uses WAGE ~ EDUCATION
Extras - AI does a bayesian comparison

## Citations
The manual portion of this reposotiory was created following the SciPy guide: https://scipy-lectures.org/packages/statistics/index.html


