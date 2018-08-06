# Multiple-Linear-Regression
Demonstration of developing a  model which would derive the relationship between the output and input data this is a similar case of
linear regression but in this case, we have more than one variable which is contributing to the output. Consider the following diagram.<br>

![Model](1.png)

As we have multiple variables sometimes we have numerical values like salary, age while sometimes have text days like the name of the city, name of the guide and many more. So how to handle those data well we create dummy variables for example in the below diagram we have a situation where we have two type of cities so to represent one we would use 1 while for another we would use 0. We can just use a different variable for city two because of many problems which can arise due to creating more dummy variable like in this one instead of using another variable for another city we can just use (d1-1). For more detail, I'll add more exams in the future so let's build a model which can do this.<br>

![Dummy Variable](2.png)

5 methods of building models
1. All-in :
    In this step, we just provide the data to the model without taking care of the variable or the number of dummy variables.
2. Backward Elimination [FASTEST METHOD]
    1. Select a significance level to stay in the model.
    2. Fit the full model with all possible predictors.(predictor = variables).
    3. COnsider the predictor with the highest P-value.
    4. Remove the predictor.(Carefully reomove the variable cause the removal affects the whole equation).
    5. Fit model without this variable.
3. Forward Selection
    1. Select a significance level to enter the model.
    2. Fit all simple regression models y~xn Select the one with the lowest P-value.
    3. Keep this variable and fit all possible models with one extra predictor added to the one you already have.
    4. Consider the predictor with the lowest P-value.
4. Bidirectional Elimination
    1. Select a significance level to enter and to stay in the model.
    2. Perform the next step of forward selection.
    3. Perform All steps of backward Elimination.
    4. No new variables can enter and no old variables can exit.
    
    If we have 10 columns then we would have 1023 combinations models.
    
    
