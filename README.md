# ST362_Project
**Members**

Garrett Stover - 210165190

Graham Nicholls - 

**Description:**

Governments have been around almost since the beginning of humanity, and politics even before that. The way people live is dictated by the society and system they live in, and is extremely important to their way of life. Despite this, many are often suspicious of their government’s actions, with good reason. Numerous scandals and crimes have been exposed over centuries worldwide, each increasing distrust in their respective governments. What we wanted to see was if distrust in governments and the degree to which people are free had anything to do with how skeptical people are. Using the World Happiness Index from 2016 and making a few changes to observations, we produced a model to compare skepticism, using trust in government, freedom, and region of each nation.

**The Variables:**

Name: Name of the country

Region: Region the country belongs to

Happiness Rank: Rank of the country based on the Happiness Score

Happiness Score: A metric measured in 2016 by asking the sampled people the question: "How would you rate your happiness on a scale from 1 to 10?”

Economy (GDP per Capita): GDP of the country

Family: Index of family involvement and community

Health (Life Expectancy): Average life expectancy

Freedom: The extent to which citizens are free 

Trust (Government Corruption): The extent to which Perception of Corruption in government

Generosity: The extent to which Generosity contributed to the calculation of the Happiness Score

Skepticism: An index of the general skepticism that the citizens express

**Changes:**

Outside of the model, the only change to the actual variables made was the Region variable. Before the change, there were 10 different regions from around the world, which were Western Europe, Central and Eastern Europe, Eastern Asia, Southeastern Asia, Southern Asia, Middle East and Northern Africa, Sub-Saharan Africa, North America, Latin America and Caribbean, and Australia and New Zealand. However, we felt that these regions could be renamed and combined into larger subregions that would allow us to create one of the features for our model. The new regions, called Europe, Asia, Africa and Middle East, Americas, and Oceania, are combinations or renaming of prior regions:

Western Europe, Central and Eastern Europe -> Europe

Eastern Asia, Southeastern Asia, Southern Asia -> Asia

Middle East and Northern Africa, Sub-Saharan Africa -> Africa and Middle East

North America, Latin America and Caribbean -> Americas

Australia and New Zealand -> Oceania

Our second factor was related to the Freedom variable within our model. Our thoughts were that freedom most likely didn’t affect the skepticism of a person that much as freedom increased. Politicians, whether in dictatorships or in democracies, would certainly lie about their achievements, goals, or decisions, however in democracies it was much easier to discern these lies with the freedom to seek out information on the topic. Nonetheless, both a person in a dictatorship and a person in a democracy would most likely have similar skepticism toward the government. Hence, we transformed the freedom variable by using a log function to represent the minimal impact freedom would have on skepticism.

Finally, we create a high-leverage point to see the effects of such a point on our data, and to use as our third factor. We create the Vatican City, with very low freedom, low skepticism, high economy (Vatican City does have the 18th highest GDP per Capita in the world), and located in Europe, it would contrast quite a bit with the democracies around the region. One issue we knew this would have would be bad data. This was actually a positive however as we would use it to show how strong the rest of the data collected was and that it would be easy to notice such an interesting set of values for the Vatican.

Overall, our 3 factors for this project were:
  - Categorical predictor, where some of the categories have been combined after loading the data.
  - One of the predictors is log-transformed in the model.
  - Outliers in multiple dimensions

