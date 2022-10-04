# Prosper Loan Data Exploration
## by James Okoro


## Dataset

This project is an exploratory data analyses of the Prosper loan data set (https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv), provided by Udacity. The data set contains information about loan listings and related variables including borrower as well as lender information. This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.
The variables are much more than we need for this project, hence we selected 14 interesting columns, categorized them and combined two (credit grade and prosper rating) to form a new variable: credit rating. Thus, before exploration, the data set comprised 113,937 loans and 13 variables.


## Summary of Findings

In this Prosper loan data exploration, the relationship between our main variables credit rating and loan status is significant. It was observed that most of the delinquent loans have poor rating as the lowest rating HR is evident among Defaulted loan status as well as Chargedoff and there is a decline across ratings for Chargedoff and Defaulted status.

For credit rating, I also observed a strong relationship with other features such as borrower's APR, amount and income range. There is a positive correlation of borrower's APR across the ratings from AA to HR and a negative correlation for amount. Thus highly rated loans have higher amounts with lower interest rates. For income range, lower credit ratings are highly represented in lower income ranges, thus, higher income ranges show better credit ratings.

Loan status is seemingly affected by amount, stated monthly income, borrower's APR, income range and debt-to-income ratio (when we limit it to values less than 1). Most delinquent loans (Chargedoff and Defaulted) have lower loan amounts, low monthly income,  high debt-to-income ratio and lower income ranges.

From exploring other features, I verified the relationship between borrower's rate and APR to be positively correlated (correlation coefficient of 0.99). For employment status, I observed that the unemployed borrow at higher rates than all other categories of employment. Also Unemployed category have a high debt-to-income ratio and high borrower's APR. Self employed are responsible for the wide range of stated monthly income and high outliers. For Income Range, there is a positive correlation for the monthly income and a wide range of values for 100,000 above category. Also there is a negative correlation of borrower APR across the income ranges of 1-24,999 and 100,000+ which buttresses our point that the higher the income, the lower the interest rate. And as expected, income range has a positive correlation with loan amount because the higher the income, the greater the loan original amount. Most loans are 3-year termed, taken from the state of California and listed as debt consolidation. Most borrowers are listed as professionals.

## Key Insights for Presentation

This presentation is focused on the influence of four numerical loan features: borrower's annual percentage rate (APR), loan amount, stated monthly income and debt-to-income ratio on the key variables credit rating and loan status. At first, I introduced credit rating as a merged variable of credit grade and Prosper rating, then loan status. After which, I plotted their respective distributions.

I introduced the numerical variables by using boxplots. First, for credit rating against monthly income, then against debt-to-income ratio. Next, loan status was plotted against monthly income, and then debt-to-income ratio using box plots. I limited the debt-to-income ratio variable to values less than 0.5 for a clearer visualization.

Next, I plotted borrower's APR against loan status and credit rating. I also did same for loan amount using pointplot since both key variables are categorical. I ensured different color palettes were used for each quality variable to make them distinct from each plot.