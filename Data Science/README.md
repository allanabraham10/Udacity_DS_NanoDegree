# AirBnB Seattle Dataset

Medium Blog:
https://medium.com/@pa.allan10/seattle-airbnb-dataset-insights-cef8acc069e2

Installation:
Download the archive file and unardhive the datasets, then run the Jupyter notebook with the ipynb file saved in the same directory as the other data sources.

Motivation:
What is this problem that I tried to solve here?

I have done sentiment analysis on the review data and assigned a sentiment score to each listing
I have then tried adding an additional parameter to see if the price of an Airbnb has gone up, gone down or remained the same. I then combined this with other features of a listing
say number of bedrooms, bathrooms, reviews received etc and try to classify into different sentiments (Positive, negative or Neutral)

The underlying datasources comprised of the prices of airbnbs since listing, the listing details - geo, owner and ratings details and finally a review file with the comments received for each listing

Summary of Results:
Business insights that we could generate were
- The Price of an Airbnb doesn't change much with the amenities provided. This indicates that the customer eligible for the maximum facility even at cheaper prices
- The price seems to increase with the number of bedrooms and bathrooms
- The ratings have been decent in general across the price band. For the cheaper Airbnbs (under 500), even though there are quite a few low ratings, the positive ratings (8+) outweigh the negatives largely
- Over 63% customers opted for a single bedroom and amongst then a whooping 58% opted for a single bed

Acknowledgement:
I would like to express my sincere gratitude towards the instructors of Udacity who have helped me with the useful content. I would also like to thank the contributors of stack overflow, whose sharings I could look up whenever I got stuck.

File Description:
AirbnbSeattle_Udacity_Updated.ipynb - Jupyter Notebook with the codes
archive.zip - Underlying Datasources
