# Amazon_Vine_Analysis
Big Data Challenge

## Project Overview
### Purpose
The purpose of the project was to  analyze the Amazon Vine program and whether paying members for product reviews causes bias toward 5-star reviews.    The product dataset chosen to analyze was in the ‘video games’ category. 
### Process Summary
Using the cloud ETL process, the data was extracted and transformed with PySpark and loaded using an AWS RDS instance to pgAdmin. PySpark was also used to analyze the transformed data.

## Results
### Target/Filtered Data.
As seen in the filtered tables below, the target video-game reviews were first selected if more than 20 reviews, and of those,  only greater than 50% ‘helpful_votes’ were chosen.
- Over 20 ‘total votes’ filtering:



![Filter 1]( https://github.com/AlexGeiger1/Amazon_Vine_Analysis/blob/main/Resources/Picture1.png)






- Greater than 50% ‘helpful votes’ filtering:




![Filter 2]( https://github.com/AlexGeiger1/Amazon_Vine_Analysis/blob/main/Resources/Picture2.png)

### Vine vs Non-VINE Results
- There were 94 reviews in the video game category from paid Vine members and  40,471 reviews from non-Vine program members.
- 48 Vine members gave  5-star reviews while 15,663 non-Vine members’ reviews were 5-star.
- 51.06% of Vine members’ reviews were 5-star and only 38.7% were 5-star from non-Vine members.
## Summary
The results indicate there might be a positivity bias for paid reviews since about half were 5-star reviews while only about 39% of non-Vine reviews were 5-star.  
### Additional Analysis
Since only one category was chosen and the number of Vine reviews were so significantly lower than the Non-Vine reviews, selecting and combining more categories may show a more generalizable result than for just one category.
