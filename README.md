# A fee cancellation analysis

This is an analysis to understand what is causing the cancellation of plans at a gym

**IMPORTANT DISCLAIMER: the data was taken from [Hashtag Treinamentos](https://www.hashtagtreinamentos.com/?origemurl=75502579145&gad_source=1&gclid=Cj0KCQiAhomtBhDgARIsABcaYylrKGb1nVWN1YepIZrKizmVGcLsc82WnTXegQ-5H7otwLmzF1VgkPkaAsFFEALw_wcB), a company that teaches data science in Brazil, but all the project was made by my self, just took the data file and the purpose of the project.**

##  Technologies used

- Pandas: data manipulation
- Seaborn: charts
- CSV: data storage
- Sklearn: machine learning

## Investigation phase 

At this part, i just tried to understand the relationship between each column with cancellation. So this was what i found:

- **People older than 50 tend to cancel** 

![](/images/age.png)

- **If someone has more then four calls by the call center, they tend to cancel too**

![](/images/callcenter_boxplot.png) ![](/images/callcenter_bar.png)

- **More then 20 days without go to the gym also drives to a cancel scenario**

![](/images/delay.png)

- **MOST IMPORTANT ONE: Monthly plan cancellation fee was 100%**

## Forecast and Machine Learning

It was a simple model just to practice and understand a more about machine learning models.

- **Why Random Forest:** The reason that i choose Random Forest model was basically i had a classification problem, also because i've searched a couple models and Random Forest it is a more accurate algorithm than the Decision Tree and is much less subject to overfitting.

- **Tests and Accuracy:** I had a great accuracy of 99%, i guess this results are high because this is a study database.
