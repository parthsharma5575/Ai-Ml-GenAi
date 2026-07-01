# FIFA Player EDA Project

## Overview
This project presents an exploratory data analysis (EDA) of a FIFA player dataset containing 18,207 professional football players and 18 variables related to player identity, demographics, performance, club details, contracts, and financial information.[1] The goal of the project is to understand the factors that influence player value and wages, and to generate insights that can support football club decisions in recruitment, retention, and squad planning.

## Problem Statement
Football clubs need to identify valuable players, optimize transfer spending, and build balanced squads while operating within financial limits.[1] This project analyzes player attributes and financial variables to discover what drives market value and wages, identify meaningful player patterns, and support more informed decision-making.

## Business Objective
The main business objective is to help club management make data-driven decisions using player data.[1] The analysis focuses on identifying the attributes that influence value and wages, spotting cost-effective player profiles, and highlighting possible risks such as overpaid or aging players.

## Dataset Information
The dataset contains 18,207 rows and 18 columns.It includes variables such as player name, age, nationality, overall rating, potential, club, market value, wage, preferred foot, international reputation, skill moves, position, joining year, contract validity, height, weight, and release clause. Duplicate checking showed that there are no duplicate rows in the dataset.

## Data Cleaning and Wrangling
Several preprocessing steps were performed to prepare the dataset for analysis.

- A copy of the original dataset was created for safe analysis.
- Missing values in `Club` were filled with `No Club`.
- Missing values in `Value` were filled using the median, since replacing them with zero would not be appropriate.
- Missing values in `International Reputation` and `Skill Moves` were filled using the mode.
- `Contract Valid Until` was converted into datetime format for better time-based analysis.
- After cleaning, only a few null values remained in `Contract Valid Until`.

## Exploratory Analysis
The analysis was carried out using univariate, bivariate, and multivariate visualizations.

### Key findings
- Elite clubs such as Real Madrid and FC Barcelona dominate total squad market value.
- A few top clubs also account for the highest total wage bills.
- Attacking positions generally receive higher average wages than many defensive and midfield roles.
- Most players are in their early- to mid-twenties.
- Right-footed players are more common than left-footed players.
- Player wages generally increase with market value, although some players appear relatively overpaid.
- Value and wage show positive relationships with overall rating and potential.
- Only a small number of players have the highest international reputation or the highest technical skill ratings.

## Charts Included
This project includes multiple visualizations to explain player and club patterns, including:

- Top 10 clubs by total market value.
- Top 10 highest paid clubs.
- Average wage by position.
- Player position distribution.
- Preferred foot distribution.
- Age distribution.
- Overall rating vs age.
- Value vs wage.
- International reputation distribution.
- Top 20 most valuable players.
- Top 5 clubs by number of players.
- Wage distribution.
- Skill moves distribution.
- Correlation heatmap.
- Pair plot of key player attributes.

## Tools and Libraries
The project was built in Google Colab using Python libraries such as:

- Pandas
- NumPy
- Matplotlib
- Seaborn

## Conclusion
The analysis shows that player value and wages are strongly linked with performance-related attributes such as overall rating, potential, and reputation. It also highlights how clubs can use age, position, wage, and contract information to improve transfer strategy and squad balance. This project provides a strong starting point for future work such as predictive modeling, player valuation, and wage optimization.

## Suggested Future Work
- Build a machine learning model to predict player market value.
- Create wage recommendation models based on player performance and age.
- Study club-wise recruitment strategies in more detail.
- Perform contract expiry and replacement planning analysis.

## Author
**Parth Sharma**
