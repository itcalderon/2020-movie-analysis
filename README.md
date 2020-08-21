# 2020 Movie Analysis

## Introduction
The goal of this project was to provide contextual information and actionable insights to Microsoft to inform their decision about whether to join the movie production industry. We worked with four data sets from IMDb, TMDB, Box Office Mojo, and The Numbers database. However, these datasets were not complete with the necessary information needed for record linkage. As such, we gathered data through TMDB’s API and merged it with the existing data provided (IMDb, Box Office Mojo, and The Numbers) to be able to calculate profitability by genre and studio - our two primary analyses.

## Guiding Questions
1. **Which studios are the most successful along the lines of revenue, profitability, and growth?** - We wanted to get a sense of what the market currently looked like and used different metrics of studio success. The first approach that we use to answer this question is an analysis of total gross revenue by studio. We also explore profitability by studios and average percent growth in profitability in the period between 2010 and 2020.
2. **What are the most profitable genres and how have their profit potentials changed over time?** - We also wanted to explore the relationship between movie genres and profitability assuming that some genres might be associated with lower production costs and higher gross revenue potential.
3. **How might movie profitability be tied to economic conditions, specifically unemployment?** - We understand that our recommendations are based on previous data from the past 10 years and do not take into account the current state of the economy. For this reason, we decided to look into the relationship between unemployment and movie profitability during an economic contraction (i.e., financial crisis 2008-2013)

## Key Findings

1. While larger studios like Disney and Universal top the charts in gross revenue, smaller studios seem to make more profitable movies by focusing on more profitable genres.
2. According to our data, Animation, Horror, Family, Science Fiction, and Adventure were the top 5 most profitable genres from 2010 - 2019.
3. Despite a spike in profitability in 2018, most genres seem to trend downward in 2019, hinting at a larger trend within the movie industry. Thriller and Documentary movies have seen steady gains in profitability in the last few years, however.
4. There seems to be a correlation between unemployment rate and movie profitability. However, our data set was too small to definitively conclude that there is a correlation. As the unemployment rate increases, movie profitability seems to decrease.

## Recommendations
**Prioritize producing movies that tend to be more profitable** (i.e., animation, horror/thriller, and family movies). Some genres have consistently been more profitable than others. For example, horror movies seem to always be profitable. Whereas western movies seem to always result in monetary losses. 
Consider a smaller budget for initial production.

**A larger budget may not result in greater profitability.** Many smaller studios have seen great profits with smaller budgets. These studios make more profitable movies by focusing on more profitable genres. 

## Limitations & Next Steps
The main limitation encountered while carrying out this project was the size of our final data set. After cleaning our data set, we realized it was too small to thoroughly conduct the planned investigations. For example, after disaggregating our data by year and genre, we found that some years had too few entries for a given genre. This may have resulted in unreliable conclusions. To continue building on this project, we must find a larger data set to work with to build out and strengthen our genre-profitability analysis and unemployment-profitability analysis. 

Additionally, our analysis began to hint at some larger trends in the movie industry: the decline in movie theater attendance and the rise of streaming services producing their own movies. Building on this project would require gathering data to compare the profitability of streaming service productions against traditional box office productions. 

## Jupyter Notebooks & Datasets
**Studio Profitability Analayses:** studio_profitability.ipynb

**Genre Profitability Analysis:** genre-profitability-analysis.ipynb

**Unemployment Analysis:** unemployment-and-profits-analysis.ipynb

**TMDB/IMDb/BOM/Numbers dataset:** 'Cleaned Data/final_merged.csv'

**Unemployment datasets:** 'Data/UNRATE.csv' & 'Data/budgets_UNRATE.csv'

