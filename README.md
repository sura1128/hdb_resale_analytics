# hdb_resale_analytics
Analysing the resale prices of HDB apartments in Singapore between 2017-2020.

I am looking to buy an HDB resale flat. But I’m not sure what are some of the options available to me, with regards to price, location, etc. This got me thinking about doing some analysis on past trends for resale HDB flats in Singapore. I have always felt very passionate about housing because I have been renting for the past seven years (and almost ~20 years by extension if I include my childhood). 

Affordable housing for this generation of Singaporeans is a challenge because of economic conditions, the pandemic, the growth of single-person households, political environment, etc. That is what led me to do this study, in an effort to help people in similar position to be able to make more informed decisions from my insights.


<h3> Defining The Question </h3> <br>
Question 1: What is the trend of resale prices over time? <br>
-  How successful were HDB resales over 2017-2020? 
-  How expensive were HDB resale rates over 2017-2020?

Question 2: What is the trend of resale prices over time based on locations? <br>
-  How successful were HDB resales in location XYZ over 2017-2020?
-  How expensive were HDB resale rates  in location XYZ over 2017-2020?

Question 3: What is the trend of resale prices over time based on floor area (sqm)? <br>
-  How successful were HDB resales for XYZ floor area over 2017-2020?
-  How expensive were HDB resale rates for XYZ floor area over 2017-2020?


<h3> Collecting the Data </h3><br>
The data was sourced from Kaggle: [](https://www.kaggle.com/datasets/teyang/singapore-hdb-flat-resale-prices-19902020) <br>
I did an initial pass of the data on Google Sheets, and conducted some cleaning and exploratory analysis before porting it over to csv.<br>
I also added some useful columns and used these functions to achieve that: <br>
- =ROUND((N2/(O2*12)), 2) → percentage of lease left <br>
- =IFS(G2<50, "50", G2<100, "50-100", G2<150, "100-150", G2<200, "150-200", G2<250, "200-250") → category for floor area


