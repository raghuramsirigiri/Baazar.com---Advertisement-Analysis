# Baazar.com---Advertisement-Analysis
 
# Business Overview

US retailer Bazaar uses both display and search advertising running paid search ads on Google and Yahoo. Bazaar releases its ads in response to key words used by customers and are classified broadly into Branded(such as ‘Bazaar’, ‘Bazaar shoes’, ‘Bazaar clothes’ and so on) and Non Branded keywords(such as ‘shoes’, ‘dress’ that do not contain ‘Bazaar’).

Using data from Google and Bing, Bazaar’s marketing analytics team computed an ROI of 320% on their sponsored ad spending. But were skeptical because some the the user who searched bazaar might already have the intent visit Bazaar.com. This is an confusion they would like the analyst to clear. The goal is to understand the causal effect of the search ads.

__Question to be answered:__

1. What is wrong with Bob’s ROI analysis?
2. What is treatment and control in the experiment?
3. Consider First Difference Estimate and is it a good estimate?
4. Calculate  the  Difference-in-Differences?
5. What if the fixed ROI Calculation?

__Following data points were given for the data:__

1. id - ID of the search engine
2. platform - Name of the search engine
3. week  - Count of the week starting from 1
4. avg_spons - Count of clicks received form sponsored ads
5. avg_org - Count of clicks received from organic clicks

__Transformed variables:__
6. treatment - 1 for rows which are part of treatment else 0
7. post - 1 for weeks after 9 else 0
8. avg_total - Sum of click from sponsored and organic clicks

## Analysis Performed

1. Pre_post difference is calculated using the first difference approach.

2. Difference-in-Differences regression is performed to get the estimate.

# Treatment and Control Definition

## Unit of Observation
users clicking on the ads

## Treatment
Treatment is the stop of sponsored ads in Google starting from week 10.

## Control
Clicks from Yahoo, Bing and Ask are used as control
