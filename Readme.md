# Health Insurance Bill Prediction for regions of USA
This was made by me during the 6th semester(2020) for Applied Statistical Methods.<br>
A project which will help predicting the cost of the medical bills using a model implementing multiple regression.
This would be a helpful prediction analysis as healthcare costs are rising as we move ahead in time and no matter what, these costs are unavoidable.<br><br>
***Dataset Description***<br>
The dataset was obtained from Kaggle and used for this study.<br>
• No of observation (rows): 1338<br>
• Attributes (columns): 7<br><br>
Independent variables:<br>
i. age: age of the individual<br>
ii. sex: insurance contractor gender, female, male<br>
iii. bmi: Body mass index, providing an understanding of body, weights that are relatively high or low
relative to height, objective index of body weight (kg / m ^ 2) using the ratio of height to weight,
ideally 18.5 to 24.9<br>
iv. children: Number of children covered by health insurance / Number of dependents<br>
v. smoker: Smoking<br>
vi. region: the beneficiary's residential area in the US, northeast, southeast, southwest, northwest.<br><br>
Dependent variable:<br>
charges: Individual medical costs billed by health insurance<br><br>
***Approach Used in the Report***<br>
In this report I would be solving the problem with two methods using, Scikit -learn and statsmodel.<br>
• I will start by fitting the model using SKLearn. After I fit the model, unlike with statsmodels,
SKLearn does not automatically print the concepts or have a method like summary. So we have to
print the coefficients,intercepts etc. separately.<br>
• After fitting the model with SKLearn, I fit the model using statsmodels. Unlike SKLearn, statsmodels
doesn’t automatically fit a constant, so you need to use the method sm.add_constant(X) in order to
add a constant. Adding a constant, while not necessary, makes your line fit much better.<br>
• Coefficients can be obtained pretty easily from SKLearn, so the main benefit of statsmodels is the
other statistics it provides.<br>
• One of the assumptions of a simple linear regression model is normality of our data. The statistics in
the summary table in statsmodel are testing the normality of our data.<br>
• If the Prob(Omnibus) is very small, and I took this to mean <.05 as this is standard statistical practice,
then our data is not normal. This is a more precise way than graphing our data to determine if our data
is normal.<br>
• Statsmodels also helps us determine which of our variables are statistically significant through the pvalues. If our p-value is <.05, then that variable is statistically significant. This is a useful tool to tune
your model.<br>
Therefore, SKLearn has more useful features, but statsmodels is a good method to analyze your data before
you put it into your model.<br><br>
For detailed idea about the project please check the attached pdf "Multiple Regression Model" in the repository.
