# Analysis Exercise

## Goal
The goal of this exercise is to identify the most promising mobile apps from an investment point of view, using data. One way to go about this is to find apps that are experiencing an accelerating trajectory of growth and are outperforming its peers, but feel free to be creative in your approach. There are no prescribed right or wrong answers. Some facets that you may wish to consider include but are not limited to
- the number of active users, and its rate of change
- the level of engagement, e.g. as measured by average number of active days per month, or number of sessions per month, or minutes per sessions, and its rate of change

## Data
To accomplish the above goal, you will use the data included in this repo. It contains anonymized monthly app usage metrics, which has the following schema

| productId | categoryPath | startDate  | activeUsers   | avgActiveDays | totalMinutes  | totalSessions |
| -------   | --------     | -------    | -------       | ---------     | ---------     | ------        |
| 12345   | Overall > News | 2017-04-01 | 100           | 5.2           | 126           | 500           |

- `productId` : the unique identifier of a given product
- `categoryPath`: the category under which the app is registered in the app store
- `starDate`: start of the period. In this case the data is monthly, and it will be the first of the month
- `activeUsers`: the number of users that have used the app at least once during the month
- `avgActiveDays`: the average number of days in which users have used the app during the month
- `totalMinutes`: the total number of minutes of usages across all users
- `totalSessions`: the total number of sessions of usages across all users

Note that not all data points are available for every app / every month. Missing data points are some times recorded as `null`. Some months may also be missing entirely for some apps. It is up to you how you wish to handle these cases, but it is important to pay attention to these because not doing so may lead to incorrect inferences in aggregation

## Output specification
This is meant to be an open ended exercise, so the output format is somewhat up to you. However, here are some suggestions to help guide you.
- Be expansive in your ideation phases - write down any and all creative ideas you might have on how to tackle this problem, we would love to see what you come with
- Do not feel pressured to implement all of your ideas - you should not spend more than 10 hours on this exercise
- Pick one idea to implement, and tell us why you chose it

The output should include
- the code
- the thinking behind your approach
- specific recommendation of the best apps, and explanations for why you believe they are the best from an investment point of view