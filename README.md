![Statistiques](https://github.com/user-attachments/assets/a38af3db-995a-49cf-868a-97043bd223f6)

As you can see, there is a file in .pdf format. It contains the instructions. Each file in .pnb format contains a response according to the order of the instructions.
If you want reproduce exercice, the links of Data are in the ".pdf" file.

# The goal of this repository is to demonstrate my capacity to use Python on statics by mobilizing next concepts : 
- Probability Density Function ; 
- Cumulative Distribution Function ;  
- Quadratic risk and Maximum likelihood estimation ;
- Central Limit Theorem ;  
- Linear models ; 
- Point Estimation ;  
- Confidence intervals ; 
- Hypothesis tests ; 
- Resampling (Boostrapping) ;

Below are the key points to note:
# During your first practice, you may notice that manipulating "matrices" in Python (using lists or arrays) feels more like working with nested lists, not true matrices like in R.

# During the second practice, here are some good notion : 
- To visualize two subpopulations (e.g., Male/Female) in the same plot, such as a scatter plot, simply split the dataframe into two subsets and plot them together. 
- np.isclose() is used to check is two values are near the same..
- LinearRegression in scikit-learn doesn’t print a summary like R’s lm(). You have to extract values one by one: reg.coef_, reg.intercept_, reg.score(X, y) ...
- If you want a full statistical summary (like in R) on regression, use statsmodels.OLS.
- To accurately estimate a distribution, we can use the following library: from statsmodels.nonparametric.kde import KDEUnivariate. For example, it's useful when estimating the probability density function (PDF) of residuals in linear regression.
- It's also useful when you want to observe the distribution of two subpopulations and the entire population together. With seaborn.kdeplot, it's difficult to plot the distributions of both Male and Female along with the overall distribution in one figure. KDEUnivariate makes this possible.

# During the third practice :
- We use pd.to_datetime to transform date to transform the nature of data to Date
- We can df.plot() to plot all quantitative variable and with there name.
- When you want to group time series, use dataframe.resample()
