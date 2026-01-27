# german-horse-racing

<meta name="robots" content="noindex">

This project applies quantitative methods, inspired by the renowned horse racing bettor Bill Benter, to predict horse race outcomes in the German market. The core of the project is the analysis notebook [`Predicting German Horse Race Outcomes using a Benter-Inspired Model`](notebooks/analysis_benter_methods.md), which leverages web-scraped data and a conditional logistic regression model to identify potential market inefficiencies. 

## Project Overview

The goal of this project is to develop a data-driven betting strategy for German horse races. We follow a similar approach to Bill Benter, who achieved remarkable success in horse race betting through statistical modeling and data analysis. 

The project involves the following key steps:

1. **Data Acquisition:** Web scraping is used to collect historical race results, horse details, jockey and trainer statistics, and betting odds from the official website of Deutscher Galopp e.V. (See the [`data_acquisition`](data_acquisition/) folder for details)
2. **Data Cleaning and Preprocessing:** The raw data is cleaned, transformed, and prepared for analysis. This also includes creating features based on domain expertise and existing literature, and handling missing values. (See the [`data_cleaning`](data_cleaning) and [`data_processing`](data_processing) folders)
3. **Model Building:**  A conditional logistic regression model is trained on the processed data to predict the probability of each horse winning a race.  
4. **Model Evaluation & Betting Strategy:** The model's performance is evaluated on unseen data, and a simple betting strategy is implemented based on the model's predictions. The strategy's profitability is assessed through backtesting and statistical analysis.  (See the [`notebooks`](notebooks) folder for steps 3 and 4)

## Key Features

The model incorporates a variety of features related to horses, jockeys, trainers, and race conditions, including:

* Horse's past performance (strike rate, speed ratings, earnings)
* Jockey and trainer statistics
* Starting stall position
* Horse's handicap rating
* Betting odds

Results: The strategy achieved a statistically significant outperformance (p-value: 0.02) against the parimutuel takeout in backtesting.

## Repository Structure

* `data`: Contains the raw, processed, and additional datasets used in the analysis.
* `data_acquisition`:  Includes scripts for web scraping the horse racing data.
* `data_cleaning`: Contains scripts for cleaning the raw data. 
* `data_processing`: Includes scripts for preprocessing the data, feature engineering, and data transformation.
* `documentation`: May contain additional documentation or reports related to the project.
* `notebooks`: Houses the main analysis notebook [`Predicting German Horse Race Outcomes using a Benter-Inspired Model`](notebooks/analysis_benter_methods.md).

## How to Use

1. Clone the repository to your local machine.
2. Ensure you have the required R and python packages installed (see the scripts and notebooks for details).
3. Open and run the [`Predicting German Horse Race Outcomes using a Benter-Inspired Model`](notebooks/analysis_benter_methods.md) notebook to reproduce the analysis and explore the results.



