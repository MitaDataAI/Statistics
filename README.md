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
# Programm 1

## During your first practice, you may notice that manipulating "matrices" in Python (using lists or arrays) feels more like working with nested lists, not true matrices like in R.

## During the second practice, here are some good notion : 
- To visualize two subpopulations (e.g., Male/Female) in the same plot, such as a scatter plot, simply split the dataframe into two subsets and plot them together. 
- np.isclose() is used to check is two values are near the same..
- LinearRegression in scikit-learn doesn’t print a summary like R’s lm(). You have to extract values one by one: reg.coef_, reg.intercept_, reg.score(X, y) ...
- If you want a full statistical summary (like in R) on regression, use statsmodels.OLS.
- To accurately estimate a distribution, we can use the following library: from statsmodels.nonparametric.kde import KDEUnivariate. For example, it's useful when estimating the probability density function (PDF) of residuals in linear regression.
- It's also useful when you want to observe the distribution of two subpopulations and the entire population together. With seaborn.kdeplot, it's difficult to plot the distributions of both Male and Female along with the overall distribution in one figure. KDEUnivariate makes this possible.

## During the third practice :
- We use pd.to_datetime to transform date to transform the nature of data to Date
- We can df.plot() to plot all quantitative variable and with there name.
- When you want to group time series, use dataframe.resample()
- To implement linear regression, we need to create an instance of the model and then apply it to our data. A basic understanding of object-oriented programming is necessary to fully grasp this process.

## During the fourth practice :
- To visualize the correlation between all variables, we can use Pandas’ corr() method to compute the correlation matrix, and Seaborn’s heatmap to plot it.
- Seaborn’s pairplot becomes quickly limited when dealing with many variables. It is more suitable for exploring relationships between the target variable and a few selected features.
- Additionally, we can use Pandas to plot distributions, helping us create more ergonomic and focused visualizations.

# Programm 2

# Programm 3 : ROBOT

## Question 1 to 9
- It is good practice to store features X and target y as NumPy arrays. This makes them- easier to use with scikit-learn.
- Before applying linear regression, we should normalize the features. The target does not need to be normalized.
- After normalization, the mean of each feature should be close to zero.
- Linear regression does not work well with very high-dimensional data.
- There is no clear rule for how many features are "too many", so it is helpful to try PCA first.
- We can compare the results of linear regression with and without PCA.
- It is also useful to select features using LASSO regression (we will see this later).
