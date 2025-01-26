#  Airbnb Europe Exercise
### Exploratory Data Analysis report
---
[Here](https://docs.google.com/spreadsheets/d/1ecopK6oyyb4d_7-QLrCr8YlgFrCetHU7-VQfnYej7JY/edit?usp=sharing) is the link to the dataset that has been analysed for this report. [Here](https://www.sciencedirect.com/science/article/pii/S0261517721000388) is the link to the corresponding paper.

In this report i will go through the findings i had answering the questions from the task sheet. The corresponding code is found in the notebook in this repository.

### Exploratory questions

1 -  How many listings are in each city in total and also per type of day?
| city | listings |
| ----------- | ----------- |
|london|       9993|
|rome|9027|
|paris|6688|
|lisbon|5763|
|athens|5280|
|budapest|4022|
|vienna|3537|
|barcelona|2833|
|berlin|2484|
|amsterdam|2080|
2 - Which city has the biggest proportion of superhosts?
|City|Superhost_proportion|
| ---------|--------|
|athens|42%|

3 - Which cities have listings with more than four rooms?

Cities with listings with more than four rooms are amsterdam, berlin, barcelona, lisbon, london, paris, rome

4 - Which city has the most entire home/apt type listings?

Rome has the most entire home/apt type listings with 5561

5 -  Are ratings typically high across listings, or is there a wide variation?

Ratings are usually high, ratings below 60 are very unusual. The mean value is roughly 92.6


6 - How does person_capacity vary across listings? What is the most common capacity of listings?

The most common person capacity in airbnbs is two people. Interestingly, there are no listings with a person capacity of only one person. The maximum person capacity is six. From the values from two to six, every capacity is fairly common and occurs in more than 2,000 listings

7 - Plot the distribution of realSum for both weekday and weekend offers. Is it normally distributed, skewed, or multimodal? If skewed, consider using transformations (e.g., log transformation) to normalize it.

The price distribution has been analyzed through the use of a logarithmically scaled histogram. In this it was visible that the price is in a multimodal distribution. In the lower price area skewed characteristics are visible, with most prices being on the lowest end of the spectrum. 

The other maxima differentiate depending on whether the listing is for weekend or weekday stays. Although, we see two maxima in both distributions, which contain much higher prices on the weekend.


9 - Examine the distribution of cleanliness_rating.

The cleanliness ratings are distributed very similarly to the overall guest satisfaction. Ratings below 6 are very unusual. The average value is a little higher with ~9.39. The distribution is skewed with the maximum on the highest cleanliness rating of 10.

### Testing questions

1 - Is there a difference in price between two cities? Choose at least three pairs of cities during weekdays.

Amsterdam and Berlin: I compared these capitals as i thought their position on the continent and country GDP per capita are comparable.
Results:
amsterdam:
545.0205264394499
berlin:
240.22042165722016
Surprisingly, the price of listings in Amsterdam seems to be double the price of listings in Berlin.

Rome and Barcelona: I compared these cities as they are both mediterranean and quite touristic
Results:
rome:
201.6180532991999
barcelona:
288.3916670664095
Airbnbs in Barcelona seem to be on average 50% more expensive than airbnbs in Rome.

London and Budapest: I compared these cities as they are both on different sides of the continent.
Results:
london:
360.2303477719071
budapest:
168.4293673444308
Costs of Airbnbs in London are double the average costs of airbnbs in Budapest.

2 - Does the price tend to be higher on weekends?

On average, the price on weekends is 8.28€ higher.

3 - Are listings of superhosts more expensive than those of normal hosts?

The opposite is the case, listings of superhosts are on average 34.18€ less expensive.

4 - Are superhosts closer to the city center and metro station than normal hosts?

Superhost listings are on average roughly 300m closer to the city center and on average 1.42m closer to the next metro station. The difference in average distance to the next metro station seems neglectable.

5 - Are superhosts cleaner than normal hosts?

The cleanliness rating of superhosts is on average 0.596 points higher. This seems like a relevant difference, if we put into account that appartments are in general usually reviewed as very clean.

6 - Is there a pattern between room types and superhost status?

Superhosts seem to be more likely to rent out entire homes/apts and a lot less likely to rent out shared rooms

7 - Is renting an entire home/apt more expensive than a private room? Does that depend on the city?

Entire homes and appartments are on average more expensive than private rooms in all cities. 
Private rooms are also usually more expensive than shared rooms, an exception is Budapest, where shared rooms are on average more expensive than private rooms.
In cities which are on average more expensive in all room types, the price gap between entire homes/apts and the other room types is also bigger than in cities where the average listing is cheaper.

8 - Create a map for each city where the top 10 most expensive Airbnbs are shown and the top 10 cheapest Airbnbs are shown.

See notebook for graphs and images used for this analysis.
