# ANOVA: Penguins' Flipper 🐧📊

This project explores the differences in flipper lengths across three species of penguins: **Adelie**, **Gentoo**, and **Chinstrap**, using the **Palmer Penguins** dataset. Through **ANOVA (Analysis of Variance)**, we determine whether there is a statistically significant difference in the flipper lengths among the species. 

## Introduction

The [**Palmer Penguins** dataset](https://www.kaggle.com/datasets/larsen0966/penguins) provides an alternative to the well-known Iris dataset for data visualization and statistical analysis. In this project, we focus on the **flipper lengths** of three penguin species: **Adelie**, **Gentoo**, and **Chinstrap**.

The key objective of the project is to test whether the mean flipper length varies significantly between species, using **one-way ANOVA** followed by **post-hoc Tukey's HSD test** to identify where the differences lie.

## Installation

To get started with this project, you'll need to have **R** installed on your local machine.

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ANOVA-penguins-flipper.git
   cd ANOVA-penguins-flipper
   ```

2. Install required R packages by running the following in your R console:
   ```R
   install.packages(c("dplyr", "ggplot2", "readr", "car", "multcomp"))
   ```

## Usage

1. Open the **AOL-Penguin.Rmd** file in **RStudio**.
2. Run the entire markdown file to perform the ANOVA analysis, check model adequacy, and view visualizations.
3. Alternatively, view the preprocessed dataset (**penguins_preprocessed.csv**) and presentation slides (**results-PPT.pdf**) for a quick overview of the results.

## Project Results

The ANOVA results show a significant difference in the mean flipper length across the three penguin species. The p-value obtained from the ANOVA test was much lower than the significance level of 0.05, indicating a significant difference between at least one pair of species.

### Conclusion:
Since the acquired p-value is less than **0.05**, we reject the null hypothesis and conclude that there is a significant difference in the flipper lengths of at least one penguin species. 

The **Tukey's HSD test** further revealed the following differences between species:
- **Gentoo** penguins have significantly longer flippers than both **Adelie** and **Chinstrap** penguins.
- **Chinstrap** penguins have slightly longer flippers than **Adelie** penguins, but the difference is less pronounced.
