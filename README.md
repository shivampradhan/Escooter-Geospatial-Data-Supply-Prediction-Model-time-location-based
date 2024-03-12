# Task

The goal of the task is to understand your strengths in the data science process. The home task consists of a problem that is similar to our day-to-day work. We will share a synthetic dataset with you and a task description, and we expect you to submit a rendered notebook showing your work. 

 

We will evaluate:

The quality of your exploratory data analysis
The coherence and structure of your ideas and code
Your modeling approach, training, and validation methodology
The applicability of your modeling technique to the real-life task you are trying to solve
Your take on how the impact of the model should be evaluated in real-world interactions with our user base 
Please find the introduction to the task here:

 

Efficient supply allocation

The success of Bolt as a ride-hailing platform depends on a marketplace or efficient matching supply and demand in real-time. There are two sides in a ride-hailing marketplace: riders (demand) and drivers (supply). One of the challenges that we aim to solve is efficient supply allocation, so riders can always get a ride and drivers have stable earnings. Knowledge about how demand changes over time and space is crucial to comprehend supply dynamics. 

 
 The source data is approximately 630000 rows of synthetic ride demand data which resembles the real-life situation in the city of Tallinn:

    start_time - time when the order was made
    start_lat - latitude of the order's pick-up point
    start_lng - longitude of the order's pick-up point
    end_lat - latitude of the order's destination point
    end_lng - longitude of the order's destination point
    ride_value - how much monetary value is in this particular ride


For this test task we expect you to:

* Explore the data and suggest a solution to guide the drivers towards areas with higher expected demand at given time and location
* Build and document a baseline model for your solution
* Describe how you would design and deploy such a model
* Describe how to communicate model recommendations to drivers
* Think through and describe the design of the experiment  that would validate your solution for live operations taking into account marketplace specifics

The goal of the task is to understand your strengths in the data science fundamentals and product thinking.

Data for the task:
The source data is approximately 630000 rows of synthetic ride demand data which resembles the real-life situation in the city of Tallinn:

start_time - time when the order was made
start_lat - latitude of the order's pick-up point
start_lng - longitude of the order's pick-up point
end_lat - latitude of the order's destination point
end_lng - longitude of the order's destination point
ride_value - how much monetary value is in this particular ride
Please do not spend more than 8 hours on this task.

Please describe what additional data would you consider useful and cite the main references used in your solution, if any.
Solve the task in Python and present it in a rendered Jupyter notebook exported as html, please upload it on the link as zip file.

# Introduction 

1. Exploration
- importing library
- loading data
- EDA
- data cleaning
- visualisation of columns
- lat long plots
- key start locations

2. Feature Engineering
- total displacment
- day , hour, month
- district
- time of the day
- time of the day vs total displacement

3. Clustering analysis
- by ride value (k means)
- by displacement (didnt give good results)

4. Predictive Modelling 

a. by district and subdistict data
- data creation 
- racing bar graph for district vs day
training arima , random forest , linear regression , ridge lasso regression model
- exporting model

b. by density based clustering
- creating data
- DBSCAN
- training model on cluster data 
- exporting model

other analysis & answering questions 
## Solution is in the ipyb file
