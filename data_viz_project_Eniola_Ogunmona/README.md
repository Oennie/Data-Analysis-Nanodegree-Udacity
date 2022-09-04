# Loan Data Exploration



## Dataset

The data set contains 113,937 loans with 81 variables on each loan, including loan amount, interest rate, current loan status, borrower income.

## Summary of Findings

In the exploration, I looked at the distribution of the different variables and relationships between them. Here is what I found
> * Most of the loans are currently running and completed. A few loans are charged off, defaulted, past due, cancelled or final payment been made
> * Most of the original loan taken fall a little below 5000
> * The borrower (interest) rate charged is between 0-0.5. The distribution of borrower rate is right skewed and unimodal in nature
> * Monthly loan payment has a positive relationship with loan original amount while borrower rate has a negative relationship with original loan amount
> * The distribution between loan status (cancelled) and loan original amount has a wide density function with most of the values occuring between 0 - 5000 which could imply that lower amount of loans taken are more likely to get cancelled.
> * Those with higher ratings (AA-B) could have access to higher loan amounts than the other ratings
> * The income range relating to the loan original amount has more frequency in loans taken by those with low income ranges (\\$0 - $49999), unemployed or didn't disclose income info over those with higher income ranges (\\$50,000-100,000+)
> * The relationship between credit grade and loan status on loan original amount helps understand  their distribution.

## Key Insights for Presentation

For the presentation, I focus on exploring the following variables and their relationship with each other; the original amount of the loan, borrower rate, monthly loan payment, range of income and credit grade. I start by introducing the
loan status variable, followed by the distribution of loan original amount and borrower rate on a logarithmic scale.

I then look at the relationship between borrower rate and loan original amount on a heat map, the relationship between monthly loan payment and loan original amount on a logarithmic scale. I then look at the categorical variables (loan status, credit grade, income range) in relation to loan original amount on a violin plot. Finally, I take a look at the relationship between credit grade and loan status on loan original amount.
