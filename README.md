Project Overview

An analysis of films released between 2015 and 2020 combining IMDb and Metacritic data to explore whether director gender is associated with critic and audience reception.

Research Questions:
Do female-directed films receive different critic scores?
Do audience ratings differ?
Are there budget differences?
Does director gender influence ROI?
Can sentiment analysis of movie descriptions predict critic reception?

Tools Used:
Python
Pandas
MongoDB
Scikit-Learn
Transformers
Seaborn
Matplotlib

Visualizations

<img width="563" height="453" alt="image" src="https://github.com/user-attachments/assets/37f15d34-c3b7-429e-a506-8c9ed8044d32" />

<img width="846" height="545" alt="image" src="https://github.com/user-attachments/assets/53f6f39a-f75e-40e8-9140-2667aaf0c915" />

<img width="842" height="545" alt="image" src="https://github.com/user-attachments/assets/08361756-6443-4c02-b07d-2b29f24e6279" />

<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/d30182b9-98a0-456e-85ae-771daa47f329" />

Conclusions

This project examined differences between female-directed and male/other-directed films released in 2019 using data from IMDB and Metacritic. The datasets were merged and analyzed using descriptive statistics, machine learning sentiment analysis, and regression modeling.

The results showed that female-directed films received substantially higher critic scores than male/other-directed films. Audience ratings were generally similar between the two groups, while female-directed films tended to be produced with smaller budgets. In the 2019 dataset, female-directed films also demonstrated a higher average return on investment.

Regression analysis confirmed that director gender was significantly associated with critic scores. Female-directed films scored approximately 10 points higher on Metacritic on average. Sentiment analysis of movie descriptions did not significantly improve the model, suggesting that plot description sentiment was not a strong predictor of critic reception. The sentiment model appeared to capture the tone of movie descriptions rather than the quality or reception of the films themselves.

As an additional validation step, the analysis was expanded to include films released between 2015 and 2020. The broader dataset showed that higher critic scores and smaller budgets for female-directed films remained consistent across multiple years, while the ROI advantage observed in 2019 was less consistent. This suggests that 2019 may have been an especially strong year for female-directed films rather than evidence of a long-term profitability advantage.

A genre-level analysis provided additional context for these findings. When films released between 2015 and 2020 were grouped by genre, female-directed films received higher average Metacritic scores in 20 of 22 genres. Higher scores were observed not only in dramas and documentaries, but also in genres traditionally associated with male directors, including action, crime, science fiction, horror, and war films. Only the fantasy and family genres showed a small advantage for male/other-directed films. This suggests that the higher critic scores associated with female-directed films were not driven by a single genre, but were broadly distributed across many types of films.

While this analysis does not establish a causal relationship between director gender and film quality, it does suggest that female-directed films consistently achieved strong critical reception across a wide range of genres despite generally having smaller production budgets.

Overall, this project demonstrates how combining multiple data sources, machine learning techniques, statistical modeling, and data visualization can be used to explore patterns in movie performance and critical reception.
