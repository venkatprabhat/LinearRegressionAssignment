# Project Name
A bike-sharing system offers bicycles for shared use on a short-term basis, either for a fee or free of charge. Many of these systems feature computer-controlled docking stations where users can input payment details to unlock a bike. Once borrowed, the bike can be returned to any docking station within the same network.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
A US bike-sharing provider has experienced significant revenue declines due to the ongoing COVID-19 pandemic. Struggling to remain competitive, the company has decided to create a strategic business plan to boost revenue as soon as the lockdown ends and the economy recovers.

In preparation for the post-quarantine market, the company seeks to understand the demand for shared bikes among the public. This insight will allow them to better meet customer needs, differentiate themselves from competitors, and generate substantial profits.

The company aims to identify:
- The key variables that significantly predict the demand for shared bikes.
- How effectively these variables explain the fluctuations in bike demand.

### Business Goal:
The objective is to develop a model that predicts the demand for shared bikes using the available independent variables. This model will help management understand how demand changes with different features, enabling them to adjust their business strategy accordingly. By doing so, the company hopes to meet demand levels and fulfill customer expectations. Additionally, the model will provide valuable insights into the demand dynamics in new markets.

To achieve this, the company is performing multiple linear regression on the Boombikes bike rental dataset. The goal is to predict the number of bike rentals based on various independent factors such as temperature, weather conditions, humidity, holidays, and more. This analysis will guide the company in navigating the post-pandemic market with informed decisions.

## Technologies Used
- numpy
- pandas
- seaborn
- matplotlib
- statsmodels
- sci-kit learn

## Conclusions

- The R-squared value for the training set is 83.29%, while the test set value is 80.7%. This suggests that the model explains a significant portion of the variance in the test set, indicating it is a reliable model.
  
- The mean squared error (MSE) of the developed model is nearly zero on both the training and test datasets, indicating that the variance is predicted accurately for the test set.

- Significant variables were selected using p-values and Variance Inflation Factor (VIF). Additionally, Recursive Feature Elimination (RFE) was conducted for automated variable selection.

- The major steps included in the Python notebook were data interpretation, visualization, preprocessing, model training, feature selection, residual analysis, and model evaluation on the test set.

- Key concepts like Exploratory Data Analysis (EDA), p-values, VIF, and RFE were used in the model-building process, which was carried out using the `statsmodels` library.

### Analysis from the Model:

- **When the Demand is High:**
  - **Seasonal Peaks:** Bike rentals increase year over year, with the highest demand occurring between May and October due to favorable weather and outdoor activities.
  - **Fall Season:** Peak demand is observed during the fall season, likely due to milder temperatures and consistent weather.
  - **Weather Conditions:** Rentals are significantly higher on clear or partly cloudy days, as people are more inclined to rent bikes in pleasant weather.
  - **Weekends and Holidays:** There is a slight increase in bike rentals on weekends and holidays, as people take advantage of their free time for leisure activities.
  - **Ideal Temperature:** Moderate temperatures drive the highest demand, as extreme weather conditions (too hot or too cold) negatively affect rental rates.

- **When the Demand is Low:**
  - **Spring Season Decline:** Bike demand decreases during the spring season, potentially due to less predictable or inconsistent weather conditions.
  - **Severe Weather Conditions:** No bikes are rented during heavy rain, thunderstorms, or snow, as these conditions pose safety risks and deter users.
  - **Light Rain and Snow:** Even light rain or snow leads to a reduction in bike demand, although the drop isn't as sharp as during severe weather.
  - **High Winds:** Strong winds negatively impact bike rentals, making rides more difficult and less enjoyable.
  - **Extreme Temperatures:** Both extreme heat and cold lead to lower rentals, as harsh weather conditions discourage outdoor activities.


## Acknowledgements
- [References](https://github.com/ContentUpgrad/Linear-Regression)


## Contact
Created by [@venkatprabhat] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
