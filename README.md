# Formula 1 Pit Stop ANOVA Project

This project analyzes Formula 1 pit stop performance using ANOVA methods to understand how pit stop times vary across teams, racing generations, and race locations. Pit stops are a major part of race strategy, where even small differences in time can affect position and overall race outcomes.

The main goal of this analysis is to answer the following research question:

**Do Formula 1 pit stop times differ by team, racing generation, and/or track location, and does team performance change differently across generations?**

To address this question, a factorial ANOVA model was used to evaluate:

- Differences in mean pit stop times across teams
- Differences in mean pit stop times across racing generations
- Differences in mean pit stop times across track locations
- Interaction effects between team and generation

The dataset contains Formula 1 pit stop information, including:

- Pit stop duration/time
- Team/Car
- Race year
- Race location
- Race identifier
- Lap and stop number

Before running the analysis, the pit stop time variable was cleaned and converted into numeric seconds. Invalid pit stop times were removed, and extreme outliers were excluded so the analysis focused on realistic pit stop performances. Because the dataset was unbalanced, Type II sums of squares were used in the ANOVA model. A log transformation of pit stop time was also used to improve the residual diagnostics.

## Key Features

- Cleaning and preprocessing Formula 1 pit stop data
- Converting pit stop time into a usable numeric response variable
- Creating racing generation groups from year ranges
- Applying a factorial ANOVA model with team, generation, and track location
- Using Type II sums of squares for an unbalanced dataset
- Testing whether pit stop times differ across teams
- Testing whether pit stop times differ across racing generations
- Testing whether pit stop times differ across track locations
- Testing whether team performance changes across racing generations
- Using Tukey post-hoc comparisons to examine specific group differences
- Using visualizations to compare pit stop distributions by team, generation, year, and track location
- Interpreting results using course based ANOVA methods

## Results Summary

The ANOVA results showed that pit stop times differed significantly across teams, racing generations, and track locations. The generation effect was the strongest effect in the final model, suggesting that broader changes in Formula 1 regulations, technology, equipment, and pit crew methods had the largest impact on pit stop performance over time.

The race or track location effect was also significant, meaning pit stop times were not identical across locations. This suggests that pit stop performance is influenced by track specific conditions such as pit lane layout, race context, and strategy differences.

The team effect was significant as well, showing that pit stop times differed across constructors. The interaction between team and generation was also significant, meaning team performance did not change at the same rate across the two racing eras. In context, this suggests that pit stop performance is shaped by broad Formula 1 development, track-specific conditions, and each team’s ability to adapt across eras.

## Project Purpose

This project demonstrates how ANOVA can be used to analyze race performance data. The analysis connects statistical testing with a practical racing questions by examining whether differences in pit stop performance are related to team, racing generation, track location, and interaction effects.

This project also demonstrates:

- Real-world data cleaning
- Statistical hypothesis testing
- Factorial ANOVA interpretation
- Analysis of main effects and interaction effects
- Use of post-hoc comparisons
- Comparing group means across multiple categorical variables
- Data visualization for statistical results
- Connecting statistical output to meaningful Formula 1 context

## Future Improvements

Future versions of this project could include additional seasons, more detailed regulation periods, and combining teams that changed names across generations. The analysis could also include more detailed track specific variables, such as pit lane length, pit lane speed limit, weather, tire strategy, and race conditions, to better explain why pit stop times differ by location. The project could also be extended with regression or machine learning models to predict pit stop time using additional variables such as lap number, race, stop number, driver, season, and circuit characteristics.

Dataset link: https://www.kaggle.com/datasets/jtrotman/formula-1-pitstops-1994-2010
