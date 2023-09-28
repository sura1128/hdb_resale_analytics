# hdb_resale_analytics
Analysing the resale prices of HDB apartments in Singapore between 2017-2020 (WIP: dataset to be updated with 2021-2023).

I am looking to buy an HDB resale flat. But I’m not sure what are some of the options available to me, with regards to price, location, etc. This got me thinking about doing some analysis on past trends for resale HDB flats in Singapore. I have always felt very passionate about housing because I have been renting for the past seven years (and almost ~20 years by extension if I include my childhood). 

Affordable housing for this generation of Singaporeans is a challenge because of economic conditions, the pandemic, the growth of single-person households, political environment, etc. That is what led me to do this study, in an effort to help people in a similar position to be able to make more informed decisions from my insights.


<h2> Defining The Questions </h2>

<h3> <u> A Guide To Buying an HDB Resale Flat </u> </h3>
To answer this question, we need to ask more questions and really dig into the trends over the past few years. While house hunting in a small island nation, here are a few important factors that we need to consider: <br>

-  Budget (of course, but even more so for Singapore - as this is an expensive city :D )
-  Location & neighbourhood
-  Size
-  Storey Height
-  Number of bedrooms
-  Flat model type (new generation, multi-gen, etc.) <br>

We also need to ascertain the competition for each of these criteria as there is less space and more people and everyone would want to get the best deal for themselves :)

<b> Question 1: I have a housing budget of $XYZ, am I within range to buy in the current market? What is a safe amount of buffer I can keep to make sure I am in a comfortable margin when I decide to buy my new home?</b> <br>
To be able to ascertain this, we need to study the trend of HDB resale prices over the years and determine how expensive units were in general throughout Singapore.  

<b> Question 2: I prefer a few locations which are closer to my work. But I need to also consider a neighbourhood that is young, modern and growing in the amenities I require for myself such as good restaurants, shopping malls, bookstores, etc. What are some locations I can consider? Are they within my budget? </b> <br>

<b> Question 3: As someone who is currently working from home in a hybrid work environment, I need to make sure my new home as enough space to accommodate a workspace and study. My estimation is approximately 2-3 bedrooms, to allow for guests and family members to stay over. What are some options available to me? </b> <br>

<b> Question 4: I prefer a calmer environment, far from the road and traffic, therefore I usually opt for mid-high to higher floors. Is that a viable option with my current budget? </b>

<b> Question 5: I am unaware of what kind of models are available for HDB resale flats? How do I know which one is best and most affordable for me? </b>


<h2> Collecting the Data </h2><br>
The data was sourced from Kaggle: https://www.kaggle.com/datasets/teyang/singapore-hdb-flat-resale-prices-19902020 <br>
I did an initial pass of the data on Google Sheets, and conducted some cleaning and exploratory analysis before porting it over to csv.<br>
I also added some useful columns and used these functions to achieve that: <br>
- =ROUND((N2/(O2*12)), 2) → percentage of lease left <br>
- =IFS(G2<50, "50", G2<100, "50-100", G2<150, "100-150", G2<200, "150-200", G2<250, "200-250") → category for floor area


