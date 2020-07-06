# COVID19-Urban-Sentiment-Analysis

## Abstract
In the era of digitalization, each day people leave behind their primitive lifestyles and
focus their attention on upgrading digitally however not all region are affected the same
way, considering the difference between rural and urban areas. We decided to put that
thought into question, given a specific location and timeframe bound, we investigate and
quantify the variation in both the interaction and sentiment on the internet regarding the
urban features of the region. Moreover, we made a case study on the society's mood and
behavior during the times of the COVID-19 virus, showing how much people are affected
and the way they are affected. Previous works have investigated sentiment analysis
on city events and exposure to urban areas with several methods being introduced in
analyzing them. None of them however, has been in the Middle East area nor applying
their investigations in the Arabic language. This study analyzes the activity and mood of
the Egyptian governorates on social media in terms of their urban features during the two
weeks COVID-19 was declared a pandemic and quarantine measures were taken. First
we collect all spatial and urban features regarding the Egyptian governorates to build our
own dataset along with building a dictionary of terms associated with the coronavirus
for detection. Afterwards we introduced four approaches in tweets collection regarding
locations and collected a governorate labelled corpus that would undergo our machine
learning based model for sentiment annotation. Through training and testing, our model
achieves best accuracy through normalizing and stemming the tweets, extracting both
unigrams and bigrams features and classifying using a Naive-Bayes classifier. Our results
show that Cairo, the capital, is the most interactive on social media with a total urban
land use and most population, however it also showed it was the least happy and a
significant difference in the results to the rest of the governorate which could be justified
given the highest rates in infection. It also shows that the impact of the stay at home
procedures negatively on people, halting the education on campus and remote work, but
people have been adapting given the show of a better mood through the end adding more
positivity when mentioning the virus
