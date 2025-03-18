# Statistical Modeling and Variable Selection on the `mtcars` Dataset

## Project Overview
This project involves an exploratory statistical analysis and application of regression modeling techniques using the widely recognized `mtcars` dataset in R. The primary objective is the construction of a linear regression model for predicting vehicle fuel efficiency, measured in miles per gallon (`mpg`).

## Dataset
The analysis utilizes the `mtcars` dataset, containing 32 observations and 11 key variables describing vehicle performance characteristics:

- **mpg**: Miles per gallon (dependent variable)
- **cyl**: Number of cylinders
- **disp**: Engine displacement (cubic inches)
- **hp**: Horsepower
- **drat**: Rear axle ratio
- **wt**: Weight (in 1000 lbs)
- **qsec**: Quarter-mile time (seconds)
- **vs**: Engine shape (0 = V-shaped, 1 = Straight)
- **am**: Transmission type (0 = automatic, 1 = manual)
- **gear**: Number of forward gears
- **carb**: Number of carburetors

## Methodology
The analytical approach of this project includes the following steps:

1. **Exploratory Data Analysis (EDA)**:
   - Data visualization and correlation analysis to understand relationships among variables.
   - Assessment of variable distribution and identification of potential issues such as multicollinearity.

2. **Initial Model Development**:
   - Fitting a preliminary multiple linear regression model using all available explanatory variables.
   - Diagnostic checks including residual analysis, leverage points, influence measures (Cook’s Distance), and Variance Inflation Factor (VIF) to detect multicollinearity.

3. **Variable Selection Procedures**:
   - **Forward Selection**: Incrementally adding predictors based on their statistical significance and contribution to the model.
   - **Backward Elimination**: Starting from a full model, removing variables that are least significant.
   - **Stepwise Selection**: Combining forward and backward selection methods to arrive at an optimal subset of explanatory variables.

4. **Model Refinement and Transformation**:
   - Applying polynomial transformations (such as quadratic terms) to predictors identified as important in previous selection steps.
   - Assessing improvement in model diagnostics and fit metrics after transformations.

## Tools and Libraries
- **Programming Language**: R
- **R Libraries Used**:
  - `olsrr`: For automated variable selection.
  - `car`: For regression diagnostics and multicollinearity detection.
  - `ggcorrplot`: For correlation matrix visualization.
  - `ggplot2`: For data visualization.

## Additional Information
Detailed explanations, code snippets, and visualizations are provided within the full report (available as PDF within this repository). The report includes comprehensive diagnostics, justification for chosen methodologies, and insights derived from the exploratory analysis.

\]

### Final Model Performance Metrics:
- **R-squared**: 0.886  
- **Adjusted R-squared**: 0.864  
- **AIC**: 149.38  

## Tools and Libraries
- **Programming Language**: R  
- **Libraries**: `olsrr`, `car`, `ggcorrplot`, `ggplot2`

## Note
Detailed statistical analysis, full scripts, diagnostics, and visualizations are available in the full project report (PDF format).
