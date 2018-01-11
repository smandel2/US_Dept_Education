# US_Dept_Education
College Scorecard

![alt text](https://raw.github.com/smandel2/US_Dept_Education/master/images/college_scorecard_img.png)

Goal - Predict the completion rate for first-time, full-time students at 4 year institutions within 4 years

![alt text](https://raw.github.com/smandel2/US_Dept_Education/master/images/graduation_cap.png)

Data Acquisition and Cleaning:

The data was pulled down from the U.S. Department of Education's College Scorecard via their API. I created a for loop in order to loop through the data page by page.

I dropped columns that had mostly null values and dropped rows with null values as well. Conducted some EDA on the dataset including the swarm plot below.

![alt text](https://raw.github.com/smandel2/US_Dept_Education/master/images/graduation_cap.png)


Modeling and Predictions:

![alt text](https://raw.github.com/smandel2/US_Dept_Education/master/images/graduation.jpeg)


Train, Test, Split with 33% reserved for the test set.

Ran several models including Linear Regression, GridCV with Lasso, Random Forest and a Keras model. The Linear Regression model yielded the best results.

The Linear Regression cross-predicted R2 score on the test set was 0.768. The following plot shows how well the predictions matched up to the actuals.

![alt text](https://raw.github.com/smandel2/predictions_vs_actuals.png)
