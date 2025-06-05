![Statistiques](https://github.com/user-attachments/assets/a38af3db-995a-49cf-868a-97043bd223f6)

As you can see, there is a file in .pdf format. It contains the instructions. Each file in .pnb format contains a response according to the order of the instructions.
If you want reproduce exercice, the links of Data are in the ".pdf" file.

# The goal of this repository is to demonstrate my capacity to use Python on statics by mobilizing next concepts : 
## Probability Density Function ; 
## Cumulative Distribution Function ;  
## Quadratic risk and Maximum likelihood estimation ;
## Central Limit Theorem ;  
## Linear models ; 
## Point Estimation ;  
## Confidence intervals ; 
## Hypothesis tests ; 
## Resampling (Boostrapping) ;

Below are the key points to note:
# During your first practice, you may notice that manipulating "matrices" in Python (using lists or arrays) feels more like working with nested lists, not true matrices like in R.

# During the second practice, here are some good notion : 
## When you want to vizualize two vizualize subpopulation (ex : Male/Female) in one graphic like scatter plot, you have just to separate the dataframe into two parts and present each other.
## np.isclose() is used to check is two values are proch.
## LinearRegression in scikit-learn doesn’t print a summary like R’s lm(). You have to extract values one by one: reg.coef_, reg.intercept_, reg.score(X, y) ... 
## If you want a full statistical summary (like in R), use statsmodels.OLS. 
## We need to use the next libraries to estimate precisly the distribution : from statsmodels.nonparametric.kde import KDEUnivariate. For example, when we want to estimate the Probability Density Function of residuals during linear regression, we use it.
## It is also great when we want to observe the distribution of 02 sub_population and all population. With Seaborn.kdeplot for example, it is impossible to plot the distribution of Male and Female with all child distribution. KDEUnivariate make it.

# During the third practice :
## We use pd.to_datetime to transform date to transform the nature of data to Date
## We can df.plot() to plot all quantitative variable and with there name.
## When you want to group time series, use dataframe.resample()
