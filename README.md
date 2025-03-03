  # Will the Customer Accept the Coupon?

## Overview
The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.


## Context
Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving.<br> - Would you accept that coupon and take a short detour to the restaurant?<br> - Would you accept the coupon but use it on a subsequent trip?<br> - Would you ignore the coupon entirely?<br> - What if the coupon was for a bar instead of a restaurant?<br> -  What about a coffee house?<br> -  Would you accept a bar coupon with a minor passenger in the car?<br> -  What about if it was just you and your partner in the car?<br> -  Would weather impact the rate of acceptance? What about the time of day?<br><br>
Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?


## Data
This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. <br> Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. <br> There are five different types of coupons <br> - less expensive restaurants (under 20)<br> - coffee houses<br> - carry out & take away<br> - bar <br> - more expensive restaurants (20 - $50)

The programming language used was Python, and the libraries used were: pandas, seaborn, matplotlib, numpy, random.
The specifics of the analysis, including code, visualizations, comments, and observations are contained in the following Jupiter Notebook:

[Link to Jupyter Notebook](/prompt.ipynb)

## Dataset Quality Issues

#### Missing Values:
Almost 99% of the values for 'car' column were blank. As a result, this column was dropped to reduce any deviations due to absent data.

#### Duplicate Data: 
74 duplicate rows were identified. However they have not been eliminated.

## Result Data Visualizations
![Image](/images/Coupons_By_Type.jpg)
<br>
<br>
![Image](/images/Driver_Bar_Visit_Pattern.jpg)
