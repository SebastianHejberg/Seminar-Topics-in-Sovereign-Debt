**Please Note:** 
- <font color="red">The source code for our estimation of the model by Collard, Habib, and Rochet (2015) is _**NOT**_ accessible yet.</font>



# Project Overview
Welcome to our GitHub repository. Here, we have displayed the source code for our estimation and application of the model by *Collard, Habib, and Rochet (2015)*[^1], used for the seminar *"Topics in Sovereign Debt - Spring 2024"* at the University of Copenhagen. This project includes two Jupyter Notebook files: `Data Load` and `Main Model`. Below is a brief description of each file and how they work together to achieve our project's goals.

## Data Load
The `Data Load.ipynb` file is responsible for importing and preparing data for analysis. This notebook contains:
- Data import: The process of loading data from a source CSV.
- Data cleaning: Basic data cleaning and transformation tasks, such as removing null values or correcting data types.
- Data calculation: Here, we perform simple calculations on our data and model the growth rate $g$, allowing us to derive $\mu$ and $\sigma$, among other things.

## Main Model
The `Main Model.ipynb` file is where the main analysis occurs, providing the outputs. This notebook includes:
- Model Estimation:
  - We select cases/scenarios for different maximum primary surpluses (alpha) and interest rates (time-varying or not).
  - In the main model, we run both the static and time-varying models:
    1. The static model is based on the average interest rate for the entire period and the debt-to-GDP level of 2022.
    2. The time-varying model is estimated using the country-specific MPS and constant MPS, while all other macroeconomic variables are time-varying.
- The remaining section is dedicated to list and dataframe manipulation, and the outputs are then displayed.
- Please note that to save plots locally, you need to set your own file path.
- The final section outputs the results in $\LaTeX$, but it is displayed in a dataframe format so that GitHub readers can easily understand the results.

$$~$$

### References
[^1]: Collard, Fabrice, Michel Habib, and Jean-Charles Rochet. “Sovereign Debt Sustainability in Advanced Economies”. Journal of the European Economic Association 13, no. 3 (2015): 381–420. [http://www.jstor.org/stable/24539255](http://www.jstor.org/stable/24539255). Especially supplementary materials

