# Film Industry Analytics: Director Gender, Critic Reception, and Film Performance

A data analytics and machine learning project examining relationships between director gender, critic scores, audience ratings, budgets, and return on investment using IMDb and Metacritic data.

## Key Findings

- Female-directed films received significantly higher Metacritic critic scores.
- Female-directed films were produced with smaller budgets on average.
- Audience ratings were generally similar across groups.
- Female-directed films showed higher ROI in 2019, though this pattern was less consistent from 2015–2020.
- Sentiment analysis of movie descriptions did not significantly predict critic scores.

## Research Questions
Do female-directed films receive different critic scores?<br>
Do audience ratings differ?<br>
Are there budget differences?<br>
Does director gender influence ROI?<br>
Can sentiment analysis of movie descriptions predict critic reception?<br>

## Tools Used
- Python
- Pandas
- MongoDB
- Scikit-Learn
- Transformers
- Seaborn
- Matplotlib
- Ordinary Least Squares (OLS) Regression

## Data Sources
- IMDb movie metadata
- Metacritic critic scores and movie descriptions
- Analysis focused on films released between 2015 and 2020
- Final merged dataset: 465 films

## Methodology

1. Retrieved and cleaned movie data from IMDb and Metacritic.
2. Merged datasets using movie identifiers.
3. The final analysis included 465 merged films released between 2015 and 2020.
4. Identified director gender through manual validation.
5. Performed descriptive statistical analysis.
6. Applied sentiment analysis to movie descriptions using a Hugging Face transformer model.
7. Built OLS regression models to evaluate relationships between director gender, sentiment, and critic scores.

## Skills Demonstrated

- Data Cleaning and Transformation
- MongoDB Querying
- ETL Pipeline Development
- Python Data Analysis
- Statistical Modeling
- Machine Learning
- Data Visualization
- Business Storytelling

## Visualizations

*Average Metacritic Scores by Director Gender (2019 Films)<br>*
<img width="563" height="453" alt="image" src="https://github.com/user-attachments/assets/37f15d34-c3b7-429e-a506-8c9ed8044d32" />

*Budget vs Gross Revenue (2019 Films)*
<img width="846" height="545" alt="image" src="https://github.com/user-attachments/assets/53f6f39a-f75e-40e8-9140-2667aaf0c915" />

The results showed that female-directed films received substantially higher critic scores than male/other-directed films. Audience ratings were generally similar between the two groups, while female-directed films tended to be produced with smaller budgets. In the 2019 dataset, female-directed films also demonstrated a higher average return on investment.

As an additional validation step, the analysis was expanded to include films released between 2015 and 2020. The broader dataset showed that higher critic scores and smaller budgets for female-directed films remained consistent across multiple years, while the ROI advantage observed in 2019 was less consistent. This suggests that 2019 may have been an especially strong year for female-directed films rather than evidence of a long-term profitability advantage.

*Average Metacritic Scores by Director Gender (Expanded to include 2015-2020 Films)*
<img width="842" height="545" alt="image" src="https://github.com/user-attachments/assets/08361756-6443-4c02-b07d-2b29f24e6279" />

A genre-level analysis provided additional context for these findings. When films released between 2015 and 2020 were grouped by genre, female-directed films received higher average Metacritic scores in 18 of 20 genres. Higher scores were observed not only in dramas and documentaries, but also in genres traditionally associated with male directors, including action, crime, science fiction, horror, and war films. Only the fantasy and family genres showed a small advantage for male/other-directed films. This suggests that the higher critic scores associated with female-directed films were not driven by a single genre, but were broadly distributed across many types of films.

*Metacritic Score Differences by Genre between Female-directed films and Male/other-directed films (Expanded to include 2015-2020 Films)*
<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/d30182b9-98a0-456e-85ae-771daa47f329" />

While this analysis does not establish a causal relationship between director gender and film quality, it does suggest that female-directed films consistently achieved strong critical reception across a wide range of genres despite generally having smaller production budgets.

## Regression Analysis

Ordinary Least Squares (OLS) regression was used to examine whether director gender and movie description sentiment were associated with Metacritic critic scores.

### Model 1: Director Gender

| Variable | Coefficient | p-value |
|-----------|-----------:|---------:|
| Female Director | +10.47 | 0.003 |

**Finding:** Films directed by women received approximately **10.5 higher Metacritic points** on average than films directed by male/other directors. The relationship was statistically significant.

### Model 2: Director Gender + Sentiment

| Variable | Coefficient | p-value |
|-----------|-----------:|---------:|
| Female Director | +10.19 | 0.004 |
| Neutral Sentiment | +2.10 | 0.360 |
| Positive Sentiment | -2.31 | 0.435 |

**Finding:** After controlling for sentiment classification, the effect of director gender remained nearly unchanged. Sentiment variables were not statistically significant predictors of critic scores.

### Conclusion

Female-directed films consistently received higher critic scores despite generally having smaller production budgets. This relationship remained statistically significant after controlling for sentiment extracted from movie descriptions. While the analysis does not establish causation, it demonstrates how data integration, machine learning, and statistical modeling can be used to investigate industry trends and evaluate competing explanations.


