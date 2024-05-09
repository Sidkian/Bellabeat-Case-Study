# Data Processing

The data is divided into 3 types: Daily, Hourly and by Minute

## Daily Data

We start by looking at daily level data which is in the following files:
* dailyActivity_merged.csv
* sleepDay_merged.csv

Duplicates and null records are removed and the data is merged into one csv: [daily.csv](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/daily.csv)

## Hourly Data

Hourly data is stored in the following files:
* hourlyCalories_merged.csv
* hourlyIntensities_merged.csv
* houlySteps_merged.csv

Duplicates and null records are removed and the data is merged into one csv: [hourly.csv](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/hourly.csv)

## Minute Data

Minute data is stored in the following files:
* minuteCaloriesNarrow_merged.csv
* minuteIntensitiesNarrow_merged.csv
* minuteStepsNarrow_merged.csv
* minuteMETsNarrow_merged.csv
* minuteSleep_merged.csv

Duplicates and null records are removed.

Minute sleep data is stored in: [minute_sleep.csv](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/minute_sleep.csv)

The rest is merged into one csv: [minute.csv](https://github.com/Sidkian/Bellabeat-Case-Study/blob/main/hourly.csv)