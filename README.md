# Investigating Goal Scoring Trends in Men's vs. Women's FIFA World Cup Matches

This repository contains the code and data analysis conducted to investigate whether more goals are scored in women’s FIFA World Cup matches than in men’s. The analysis focuses exclusively on official FIFA World Cup matches from January 1, 2002, onwards, excluding qualifiers, with datasets provided by DataCamp.

## Objective
The primary goal of this project is to perform a statistical analysis to determine if there is a significant difference in the mean number of goals scored in men’s and women’s FIFA World Cup matches.

## Hypotheses
Null Hypothesis (H₀): The mean number of goals scored in women's international soccer matches is the same as in men's.
Alternative Hypothesis (Hₐ): The mean number of goals scored in women's international soccer matches is greater than in men's.

## Methodology
Since the distributions of goals scored were not normally distributed, we used a non-parametric test: the Wilcoxon-Mann-Whitney U Test to compare the two datasets. This test is appropriate for data that does not follow a normal distribution and tests whether one sample tends to have larger values than the other.

## Data
`women_results.csv`: Contains match results for women's international football matches.
`men_results.csv`: Contains match results for men's international football matches.

### Each dataset includes:
- Date of the match
- Teams involved
- Goals scored by each team
- tournament information

The analysis limits the data to matches played since January 1, 2002, focusing on official FIFA World Cup matches only.

## Analysis & Results
After cleaning and filtering the data, we performed the Wilcoxon-Mann-Whitney U Test at a 10% significance level (α = 0.10). The result of the test allowed us to reject the null hypothesis, suggesting that more goals are indeed scored in women’s FIFA World Cup matches compared to men’s.

## Repository Structure
- `data/`: Contains the women_results.csv and men_results.csv files.
- `notebooks/`: Jupyter notebooks used for data analysis, including data preprocessing, exploratory data analysis (EDA), and statistical testing.
- `README.md`: Project overview and instructions on how to run the analysis.

## Requirements
- Python 3.x
- Pandas
- NumPy
- Scipy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Conclusion
The analysis provides evidence that, on average, more goals are scored in women's FIFA World Cup matches than in men's, based on the data collected since 2002. The Wilcoxon-Mann-Whitney test supports this conclusion with a statistically significant result.

## Future Work
- Extending the analysis to include other tournaments, such as continental championships.
- Investigating other factors influencing goal-scoring trends, such as team rankings or match locations.

