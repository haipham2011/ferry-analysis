# Ferry trips between Helsinki and Talinn analysis

## Description
We aim to analyze the performance of different ferry companies operating between Helsinki and Tallin using data from HRI (Helsinki Region Infoshare). Our goal is to develop a Python notebook that provides valuable insights and metrics regarding their performance.
Data link : https://hri.fi/data/en_GB/dataset/matkustaja-alusten-aikataulu-liikennointi-jasijaintitietoja-helsingin-ja-tallinnan-valilla

## Requirements

1. Data cleaning:
+ Ensure consistent date format across all columns.
+ Drop rows with missing fields.
+ Ensure consistent ship name

2. Generate a pandas dataframe with the following metrics:
+ List of available ferry names in the dataset.
+ Ferry with the highest number of trips each month.
+ Ferry that adheres the most to the departure time.
+ Ferry that adheres the most to the arrival time.

3. Create a code that generates the following plots:
+ Bar plot displaying the total number of trips for each company.
+ Plot the changes in the difference between the estimated departure time
(ETD) and the actual departure time (ATD) over time, while considering
outliers.
+ Plot the changes in the difference between the estimated arrival time (ETA)
and the actual arrival time (ATA) over time, while considering outliers. 
+ Generate a scatter plot showing the relationship between 'Sog' (Speed over
Ground) and the trip duration.
+ Create a scatter plot with a best-fit line to depict the correlation between
delay in departure (ATD - ETD) and delay in arrival (ATA - ETA). What
conclusions can be drawn about this relationship?

## How to start

1. Create a `sample_data` directory and download data from the link above
```
mkdir sample_data
cd sample_data
curl https://hri.fi/data/en_GB/dataset/matkustaja-alusten-aikataulu-liikennointi-ja-sijaintitietoja-helsingin-ja-tallinnan-valilla/resource/6750998b-c488-49c7-a303-8973a63916d6
```
2. Create virtual environment
```
python -m venv .venv
sourve .venv/bin/activate
```
3. Install dependencies
```
pip install -r requirements.txt
```
4. Run jupyter notebook script `FerryTripAnalytics.ipynb` 