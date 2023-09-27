# hdb_resale_analytics
Analysing the resale prices of HDB apartments in Singapore between 2017-2020.

I am looking to buy an HDB resale flat. But I’m not sure what are some of the options available to me, with regards to price, location, etc. This got me thinking about doing some analysis on past trends for resale HDB flats in Singapore. I have always felt very passionate about housing because I have been renting for the past seven years (and almost ~20 years by extension if I include my childhood). 

Affordable housing for this generation of Singaporeans is a challenge because of economic conditions, the pandemic, the growth of single-person households, political environment, etc. That is what led me to do this study, in an effort to help people in similar position to be able to make more informed decisions from my insights.


<h2> Defining The Questions </h2>

<h3> <u> What sort of resale HDB flat should I buy? </u> </h3>
To answer this question, we need to ask more questions and really dig into the trends over the past few years. While house hunting in a small island nation, here are a few important factors that we need to consider:
- Budget (of course, but even more so for Singapore - as this is an expensive city :D )
- Location & neighbourhood
- Size
- Storey Height
- Number of bedrooms
- Flat model type (new generation, multi-gen, etc.)
We also need to ascertain the competition for each of these criteria as there is less space and more people and everyone would want to get the best deal for themselves :)

<b> Question 1: What is the trend for resale prices over time? </b> <br>
-  How successful were HDB resales over 2017-2020? 
-  How expensive were HDB resale rates over 2017-2020?

<b> Question 2: What is the trend for resale prices over time based on locations? </b> <br>
-  How successful were HDB resales in location XYZ over 2017-2020?
-  How expensive were HDB resale rates  in location XYZ over 2017-2020?

<b> Question 3: What is the trend of resale prices over time based on floor area (sqm)? </b> <br>
-  How successful were HDB resales for XYZ floor area over 2017-2020?
-  How expensive were HDB resale rates for XYZ floor area over 2017-2020?

<b> Question 4: What is the trend of resale prices over time based on storey height? </b>
-  How successful were HDB resales for XYZ storey height over 2017-2020?
-  How expensive were HDB resale rates for XYZ storey height over 2017-2020? 

  <i>For the sake of simplicity, we have divided the story height into 3 categories:
  - High Floor = > 20 storeys
  - Mid Floor = > 9 && < 20 storeys 
  - Low Floor =  < 9 storeys</i>

Question 5: What is the trend of resale prices over time based model type? </b>
-  How successful were HDB resales of ABC flat type over 2017-2020?
-  How expensive were HDB resale rates of ABC flat type over 2017-2020? 


<h2> Collecting the Data </h2><br>
The data was sourced from Kaggle: https://www.kaggle.com/datasets/teyang/singapore-hdb-flat-resale-prices-19902020 <br>
I did an initial pass of the data on Google Sheets, and conducted some cleaning and exploratory analysis before porting it over to csv.<br>
I also added some useful columns and used these functions to achieve that: <br>
- =ROUND((N2/(O2*12)), 2) → percentage of lease left <br>
- =IFS(G2<50, "50", G2<100, "50-100", G2<150, "100-150", G2<200, "150-200", G2<250, "200-250") → category for floor area


