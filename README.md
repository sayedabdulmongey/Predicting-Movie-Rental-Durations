# Predicting Movie Rental Durations

## Project Overview

This project focuses on predicting the number of days a customer will rent a DVD based on various features provided by a DVD rental company. The goal is to build a regression model that can predict rental durations with a Mean Squared Error (MSE) of 3 or less on a test set. The dataset includes features such as rental date, return date, amount paid, rental rate, movie length, release year, replacement cost, special features, and movie ratings.

The project involves data exploration, feature engineering, and the application of regression models to achieve the desired prediction accuracy. The dataset used in this project is provided in the `rental_info.csv` file.

## Project Link

This project was originally part of the DataCamp curriculum. You can access the project on DataCamp using the following link:
[Predicting Movie Rental Durations on DataCamp](https://app.datacamp.com/learn/projects/predicting-movie-rental-durations/guided/Python)

## Dataset Description

The dataset `rental_info.csv` contains the following features:

- `rental_date`: The date and time the customer rents the DVD.
- `return_date`: The date and time the customer returns the DVD.
- `amount`: The amount paid by the customer for renting the DVD.
- `amount_2`: The square of `amount`.
- `rental_rate`: The rate at which the DVD is rented.
- `rental_rate_2`: The square of `rental_rate`.
- `release_year`: The year the movie was released.
- `length`: The length of the movie in minutes.
- `length_2`: The square of `length`.
- `replacement_cost`: The cost to replace the DVD.
- `special_features`: Any special features included with the DVD (e.g., trailers, deleted scenes).
- `NC-17`, `PG`, `PG-13`, `R`: Dummy variables indicating the movie's rating.

## Project Steps

1. **Data Import and Initial Exploration**:
   - Import necessary libraries and load the dataset.
   - Perform initial data exploration to understand the structure and content of the dataset.

2. **Feature Engineering**:
   - Calculate the rental duration in days based on the `rental_date` and `return_date`.
   - Extract dummy variables from the `special_features` column to create new features such as `deleted_scenes`, `behind_the_scenes`, `trailers`, and `commentaries`.

3. **Data Cleaning**:
   - Drop unnecessary columns such as `rental_date`, `return_date`, and `special_features`.
   - Check for and handle any missing values in the dataset.

4. **Data Visualization**:
   - Visualize the relationships between various features and the target variable (`rental_length_days`).

5. **Model Building**:
   - Split the dataset into training and testing sets.
   - Import and apply regression models to predict rental durations.
   - Evaluate the models based on their performance, aiming for an MSE of 3 or less on the test set.

6. **Model Evaluation**:
   - Compare the performance of different regression models.
   - Select the best-performing model based on the evaluation metrics.

## Conclusion

This project demonstrates the process of predicting movie rental durations using regression models. By exploring the dataset, engineering new features, and evaluating different models, we aim to achieve accurate predictions that can help the DVD rental company optimize their inventory planning.


---

Feel free to contribute to this project by submitting issues or pull requests. Your feedback and suggestions are highly appreciated!
