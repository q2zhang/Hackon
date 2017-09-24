# Hackon
Hackon day project 2017

Inspiration:
Inspired by Hackon Data's Spark program

What it does:
It uses the Spark ALS recommendation algorithm to segment customers. The algorithm segments the customers based on their predicted ratings. It finds users who have top predicted ratings for a particular item.

How I built it:
I built it using Spark SQL and Spark Data Frame with Python based on Hackon Data's Spark labs.

Challenges I ran into:
The main challenge was heavily left skewed ratings. I needed to find ways to adjust and scale them.

Accomplishments that I'm proud of:
I researched and built the model in two weeks.

What I learned:
I have found that performing training/validation/testing on a data set that is randomly split seemingly produces better results than doing so on a data set that is split based on time. However, since the time stamp is available in my data set, I believe that splitting based on time gives me more correct model. It does not make sense to use tomorrow's ratings to predict today's ratings.

What's next for Customer Segmentation Using ALS Algorithm�
The next step is to improve the recommendation performance.

Built With:
pyspark-on-databricks-plateform
