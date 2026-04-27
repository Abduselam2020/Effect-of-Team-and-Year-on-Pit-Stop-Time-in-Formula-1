# Formula 1 Pit Stop ANOVA Project

This project analyzes Formula 1 pit stop performance using ANOVA methods to understand how pit stop times vary across teams, racing generations, and race locations. Pit stops are a major part of race strategy, where even small differences in time can affect track position and overall race outcomes.

The main goal of this analysis is to answer the research question:

**Do Formula 1 pit stop times differ by team and racing generation, and does team performance change differently across generations?**

To address this question, a factorial ANOVA model was used to evaluate:

- Differences in mean pit stop times across teams
- Differences in mean pit stop times across racing generations
- Differences in mean pit stop times across track locations.
- Interaction effects between team and generation

The dataset contains Formula 1 pit stop information, including:

- Pit stop duration (full pit run, including pit entry and exit.)
- Team/Car
- Race year
- Race location
- Race identifier
- Lap and stop number

Before running the analysis, the pit stop time variable was cleaned and converted into numeric seconds. Extreme outliers and inconsistent records were removed so the analysis focused on realistic pit stop performances. The remaining dataset was then used to compare pit stop times across teams, racing generations, and track locations.

## Key Features

- Cleaning and preprocessing real Formula 1 pit stop data
- Converting pit stop time into a usable numeric response variable
- Creating racing generation groups from year ranges
- Analyzing differences in pit stop times across teams
- Analyzing differences in pit stop times across racing generations
- Analyzing differences in pit stop times across track locations
- Applying ANOVA methods to compare pit stop performance across multiple factors
- Testing whether team performance changes across racing generations
- Testing whether certain tracks are associated with faster or slower pit stop times
- Using visualizations to compare pit stop distributions by team, generation, and track location
- Interpreting results using course-based ANOVA methods

## Results Summary

The ANOVA results showed that pit stop times differed significantly across teams, racing generations, and track locations. The generation effect was especially important, suggesting that broader changes in Formula 1 technology, regulations, equipment, and pit crew methods had a strong impact on pit stop performance over time.

The team effect was also significant, showing that some teams were consistently faster or slower than others. Track location was significant as well, meaning pit stop times were not identical across race locations. This could reflect differences in pit lane layout, race conditions, circuit-specific strategy, or other track-related factors.

The interaction between team and generation was significant, meaning that teams did not all improve or change at the same rate across generations. In context, this suggests that pit stop performance is shaped by overall Formula 1 development, individual team execution, and race-location-specific conditions.

## Project Purpose

This project demonstrates how ANOVA can be used to analyze real-world sports performance data. The analysis connects statistical testing with a practical racing question by examining whether differences in pit stop performance are related to team, racing generation, track location, and interaction effects.

This project also demonstrates:

- Real-world data cleaning
- Statistical hypothesis testing
- ANOVA interpretation
- Analysis of main effects and interaction effects
- Comparing group means across multiple categorical variables
- Data visualization for statistical results
- Connecting statistical output to meaningful Formula 1 context

## Future Improvements

Future versions of this project could include additional seasons, more detailed regulation periods, and more teams. Post-hoc tests such as Tukey HSD could be added to identify which specific teams, generations, or track locations differ from each other. The analysis could also be extended with regression or machine learning models to predict pit stop time using additional variables such as lap number, race, stop number, driver, season, and circuit characteristics.
