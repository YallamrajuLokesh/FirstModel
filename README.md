# Olympic Medals Prediction

This repository contains a project aimed at predicting the number of medals won by various countries in the Olympics based on several factors such as the number of athletes, previous medals, and other attributes. 

## Dataset

The dataset consists of the following columns:
- **team**: Abbreviation of the country
- **country**: Full name of the country
- **year**: Year of the Olympics
- **athletes**: Number of athletes representing the country
- **age**: Average age of athletes
- **prev_medals**: Number of medals won in previous Olympics
- **medals**: Total medals won in the current Olympics

## Steps

1. **Data Preprocessing**
   - Loaded the dataset and filtered relevant columns.
   - Filled missing values with zeros.

2. **Exploratory Data Analysis**
   - Computed the correlation matrix to understand relationships between variables.
   - Visualized relationships using Seaborn for better insights.

3. **Model Training**
   - Split the data into training and testing sets based on the year.
   - Used Linear Regression to predict the number of medals based on `athletes` and `prev_medals`.

4. **Predictions and Evaluation**
   - Made predictions for the testing set.
   - Calculated mean absolute error to evaluate the model's performance.

5. **Error Analysis**
   - Analyzed prediction errors by team and computed an error ratio.

## Results

- The model shows a high correlation between the number of athletes and previous medals with the total medals won.
- The mean absolute error was approximately 3.54, which is below the standard deviation of medals.

## Visualizations

Visualizations were created to show the relationships between the number of athletes, previous medals, and predicted medals. 

## Conclusion

This is my first time working with machine learning and visualization, and I am excited to keep exploring and improving my skills in this field!

## Future Work

- Experiment with different regression models.
- Implement more advanced techniques like Random Forest or Gradient Boosting.
- Explore additional features that might influence medal counts.

## Installation

To set up the project, you'll need to install the required packages. You can do this using pip. Run the following command:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib
