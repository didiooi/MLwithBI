# Machine Learning with this open-source Spotfire dashboard
*Status: Incomplete*

**Didi's To-Dos**
*- Create slide deck to introduce ML and Spotfire, a BI software
- Stress importance of understanding univariate, bivariate, data transformation, data cleaning and dimensionality reduction
- Annotate each pages on Dashboard for ease of use*

## Introduction
No single data analytics is the same! Here I will provide a general guideline to help you navigate multivariate analysis. Spotfire is the next generation business intelligence tool which is free for educational and non-profit use!

## 5 1/2 Key Steps  

### 0.5 Should I transform?
Is your data clean? How clean is it? Is it too clean? Should you:
- Convert to categorical (L/M/H)  
- Do manual categorization (tags)  
- Decide what to do with outliers?  
- Make new metrics (Var1/Var2)  
- Do standard transformations? (Log/Sqrt)  
- Do Data imputation?  
- Create calculated columns? (new var)  

### 1. Univariate Patterns
Look at each variable independently and clean them up. Make variables normal by removing outliers or transforming them. Fill in missing values, if possible. Take note of “good” variables. Use your domain knowledge.  
TOOLS: Data Description, QQ Plot, Box Plots, Calculated Columns  

### 2. Bivariate Relationship
Compare two variables with regressions, ANOVA and Chi Sq. Find variables that could be strong predictors. Introduce new variables for colinear patterns -> V1/V2.  
TOOLS: Data Relationships, Scatter Plots, Box Plots  


### 3. Dimensionality Reduction
Use Principal Component Analysis (PCA is one of few DR techniques) to identify the columns with the most information and also collinearity. Find groups of columns that are *colinear* (provide the same information). Get rid of uninformative columns. You can make new metrics here.
TOOLS: PCA, Scatter Plots  

### 4. Train your Machine Learning Model
Make a training and validation set with your data. Train competing models using a straightforward algorithm - random forest. Start simple and add informative columns. Use your validation set to compare performance.  
TOOLS: RandomForest, MV Linear Regression  

### 5. Predict
Add rows to your dataset to predict using your model. Try different “scenarios” to better understand the ML model. Run sensitivity analysis on parameters.  
TOOLS: Predict, Parameter Sweep  

## Final Notes
Stay away from **confirmation bias**! Be your own critical thinker and argue against yourself. Make **data provide the proof**.  

