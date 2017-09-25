## Hackon day project 2017

* What it does: 
It uses the Spark ALS recommendation algorithm to segment customers. The algorithm segments the customers based on their predicted ratings. It finds users who have top predicted ratings for a particular item.

* How I built it:
I built it using Spark SQL and Spark Data Frame with Python based on Hackon Data's Spark labs.

* Challenges I ran into:
The main challenge was heavily left skewed ratings. I needed to find ways to adjust and scale them.

* Accomplishments that I'm proud of:
I researched and built the model in two weeks.

* What I learned:
I have found that performing training/validation/testing on a data set that is randomly split seemingly produces better results than doing so on a data set that is split based on time. However, since the time stamp is available in my data set, I believe that splitting based on time gives me more correct model. It does not make sense to use tomorrow's ratings to predict today's ratings.

* What's next for Customer Segmentation Using ALS Algorithm�
The next step is to improve the recommendation performance.

* Built With:
pyspark-on-databricks

## Dataset
[Amazon's data set](http://jmcauley.ucsd.edu/data/amazon/). provides reviews and metadate from 1996 to 2014. It contain big data sets and small data sets. I used the autotive 5-core data set which can be downloaded for this web site.


## Running on Databricks
First, you can download the data set to your computer, and then import the data set to the data bricks plateform. [Importing data](https://docs.databricks.com/user-guide/importing-data.html). After import the Python notebook, you can run the codes.


## Readings
- [Customer segmentation based on a collaborative recommendation system: Application to a mass retail company](https://www.ig.fpms.ac.be/sites/default/files/Customer%20segmentation%20based%20on%20a%20collaborative%20recommendation%20system:%20Application%20to%20a%20mass%20retail%20company_0.pdf).
- [Amazon.com Recommendations](https://www.cs.umd.edu/~samir/498/Amazon-Recommendations.pdf).
- [Collaborative Filtering](http://spark.apache.org/docs/2.2.0/mllib-collaborative-filtering.html#collaborative-filtering).

