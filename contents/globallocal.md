# Global verses Local Statistics

Compared to global statistics, local statistics more press on **where the specific patterns occur**

| Global Statistics                                          | Local Statistics                                             |
| ---------------------------------------------------------- | ------------------------------------------------------------ |
| Indentify and measure the pattern of the entire study area | Identify variation across the study area, focusing on individual features and their relationships to nearby fatures |

## Common global and local statistics

### Global spatial autocorrelation and local spatial association

The sum of LISAs for all observations is propotional to a global indicator of spatial association.





### Global regression (Ordinary least squares) and Local regression model (Geographically weighted Regression)



Global regression, also known as Ordinary Least Squares (OLS), is a statistical method used to estimate the relationship between a dependent variable and one or more independent variables. It assumes that the relationship between the variables is constant across the entire study area and uses a single set of coefficients to model the relationship. The OLS model aims to minimize the sum of the squared differences between the observed and predicted values of the dependent variable.

On the other hand, local regression, also known as geographically weighted regression (GWR), is a statistical technique that takes into account spatial variation in the relationship between the dependent and independent variables. The GWR model assumes that the relationship between the variables varies spatially across the study area, and the model estimates a different set of coefficients for each location. The GWR model uses a weighted least squares approach, where observations closer to the location being modeled have a higher weight than those further away.

#### Main differences



The main difference between OLS and GWR is that OLS assumes a global relationship between the variables, whereas GWR takes into account the spatial variation in the relationship. Therefore, GWR can provide a more nuanced and accurate model than OLS, particularly when the relationship between the variables varies across space. However, GWR can also be more computationally intensive than OLS and may require more data and a larger sample size to produce reliable results.

