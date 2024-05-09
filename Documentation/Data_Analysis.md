# Analysis

## Daily Data

The 'daily' dataframe has per day data for Total Steps, Total Distance and Distance covered during each level of activity, minutes spent on each level of activity, Calories burned and Sleep data for 33 users

The dataset doesn't give us information on what type of activity the user performed. In general, Calories burned is a good indicator of how healthy/fit a person is. However, calories can be burned by performing muscle-strengthening activities and not just by covering distance. To get a better understanding of whether the given data records muscle-strengthening activities, we can check to see how the Activity Minutes correlate to Activity Distance.

![Daily Distance vs Minutes Heatmap](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Daily%20Distance%20vs%20Minutes%20Heatmap.png?raw=true)

Here we see that Very Active Minutes is positively correlated to Very Active Distance (0.83), FairlyActiveMinutes are positively correlated to Moderately Active Minutes (0.95) and Lightly Active Minutes are positively correlated to Lightly Active Minutes (0.89).

With this, it is safe to assume that all users used their time performing activities that cover distance such as walking, jogging or running.

Now, lets see how does distance travelled translates to Calories burnt.

![Daily Total Distance vs Calories](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Daily%20Total%20Distance%20vs%20Calories.png?raw=true)

The above plots shows that Total Distance and Calories are positively correlated. This means, more calories are burned when more distance is covered. This makes sense as walking/running/jogging are good forms of exercise.

![Count of Daily Total Distance, Total Steps and Calories](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Count%20of%20Daily%20Total%20Distance%2C%20Total%20Steps%20and%20Calories.png?raw=true?raw=true)

The plots here counts the number of records in ranges for Total Distance, Total Steps, and Calories. We can see that: 
* On average, users tend to cover less than 10 Km or 15000 steps on any given day
* Average Calories burned by a user on any given day ranges between 1000 and 3000

Lets take a look at how many days do users use their fitness tracker over a month. The users are classified into 3 types based on the number of days they used their device:
* High Use: Device used for 21 to 31 days
* Moderate Use: Device used for 11 to 20 days
* Low Use: Device used for less than or equal to 10 days

![Monthly Usage](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Monthly%20Usage.png?raw=true)

From the above graphs we see that most of the users use their device for more than 21 days (88%).

To get more granular we can look at how many hours do users use their fitness tracker on a daily basis. The users are classified into 3 types based on the number of hours they used their device:
* All Day: Device used for more than 20 hours
* More than half day: Device used for more than 10 hours but less than 20 hours
* Less than half day: Device used for less than 10 hours

![Daily Usage](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Daily%20Usage.png?raw=true)

From the above graphs we see that users use their device all day a little more than half the time (57%).

We will also look at how long each user type uses their device in a day.

![Daily Usage by User Type](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Daily%20Usage%20by%20User%20Type.png?raw=true)

High Use users wear their device all day only little more than half the time (56%).
Moderate Use users and Low Use users wear it all day about 75% of the time.

Fibit devices also track sleep data.

![Total Minutes Asleep vs Sedentary Minutes and Calories](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Total%20Minutes%20Asleep%20vs%20Sedentary%20Minutes%20and%20Calories.png?raw=true)

While there is no correlation between Total Minutes Asleep and Calories burned, there is a negative correlation between Total Minutes Asleep and Sedentary Minutes.
This mean that the lesser the person sleeps the more likely they are to be sedentary and feel lazier that day.

Lets take a look at which days of the week on average do users get optimal sleep of 7 hours and optimal step count of 10000.

![Average Total Step & Total Minutes Asleep by Day of Week](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Average%20Total%20Steps%20%26%20Total%20Minutes%20Asleep%20by%20Day%20of%20Week.png?raw=true)

On average, users don't walk the recommended amount of steps everyday, which is 10000. Sundays recorded the least number of steps.
The recommended hours of sleep for an adult is 7 hours or more. On average, Sundays have recorded most amount of sleep time.

## Hourly Data

When looking at hourly data, we would like to know what hours of the day are users the most active. We can also compare data for weekdays vs weekends

![Average Total Steps by Hour of Day](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Average%20Total%20Steps%20by%20Hour%20of%20Day.png?raw=true)

From the above barplots we see that users are active between 8am and 7pm. Users cover more steps during 12pm-2pm and 5pm-7pm.
During Weekends more steps are covered between 10am-3pm.

## Minute Data

According to [Fitabase Data Dictonary](https://www.fitabase.com/media/1930/fitabasedatadictionary102320.pdf), 
"All MET values exported from Fitabase are multiplied by 10. Please divide by 10 to get accurate MET values."

Also,
* Sedentary : MET = 1.0
* Light Intensity : MET is between 1 and 3
* Moderate Intensity : MET is between 3 and 6
* Vigorous Intensity : MET > 6.0

Since this is Minute data, MET here can also be referred to as MET Minute.

The dataset consists of roughly 30 days of data. Lets group it into the following weeks:
* Week 1 = 04/11/2016 to 04/17/2016
* Week 2 = 04/18/2016 to 04/24/2016
* Week 3 = 04/24/2016 to 05/01/2016
* Week 4 = 04/24/2016 to 05/01/2016
* Week 5 = 05/09/2016 to 05/15/2016

The Total MET Minutes fo each user by week looks like:

![MET Minutes per person (Week 1)](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/MET%20Minutes%20per%20person%20(Week%201).png?raw=true)

![MET Minutes per person (Week 2)](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/MET%20Minutes%20per%20person%20(Week%202).png?raw=true)

![MET Minutes per person (Week 3)](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/MET%20Minutes%20per%20person%20(Week%203).png?raw=true)

![MET Minutes per person (Week 4)](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/MET%20Minutes%20per%20person%20(Week%204).png?raw=true)

![MET Minutes per person (Week 5)](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/MET%20Minutes%20per%20person%20(Week%205).png?raw=true)

WHO recommends a minumum 450 to 900 MET minutes per week. For additional health benifits, MET minutes per week should be greater than 900.
The most gains to be had is when the physical activity level is increased to the 3000-4000 MET minutes/ week range.

Lets take a look the users Average Weekly MET Minutes:

![Average Weekly MET Minutes per person](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Average%20Weekly%20MET%20Minutes%20per%20person.png?raw=true)

The solid yellow line represents the recommended MET minutes per week of 900. The dotted yellow lines represent the range of 3000-4000 MET minutes/week for most gains through physical activity.

To better understand users weekly MET minutes, we can classify them into groups based on avg MET minutes per week:
* Physically Inactive : < 450 MET Minutes per week
* Minumum MET minutes : 450 - 900 MET Minutes per week
* Good MET minutes : 900 - 3000 MET Minutes per week
* Best MET minutes : 3000 - 4000 MET Minutes per week
* Extra MET minutes : >4000 MET Minutes per week

![MET Minute Type Distribution](https://github.com/Sidkian/Bellabeat-Case-Study/Images/MET%20Minute%20Type%20Distribution.png?raw=true)

From the above pie chart, we see that majority of the users (45%) are in the Good MET Minute range. Only 15% are in the Best MET Minute range and 36% are in the Extra MET minute range.

For Sleep data at minute level we have values to indicate type of sleep
1 = Asleep
2 = Restless
3 = Awake

![Average Sleep Minute Distribution](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Average%20Sleep%20Minute%20Distribution.png?raw=true)

On average users sleep 384 minutes or 6.4 hours and It takes them an average of 6 minutes to fall asleep.

Lets classify users sleep log into :
* Good Sleep : 7 hours or more of sleep
* Bad Sleep : Less than 7 hours of sleep

![Sleep Distribution by Sleep Type](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/Images/Sleep%20Distribution%20by%20Sleep%20Type.png?raw=true)

We see that there is not a lot of difference in the distribution of sleep type based on Good and Bad Sleep.