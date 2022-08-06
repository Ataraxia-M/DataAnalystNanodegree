# Communicate Data Findings: Prosper Loan Dataset
## by Adeyemo Oluwatosin


## Dataset

> The dataset used for this analysis is Prosper Loan dataset. It can be downloaded via this <a href="https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv">link</a> and the data dictionary <a href="https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&source=editors&ust=1659735669445378&usg=AOvVaw3lTtSOZwDtx8iQ0HcZMa66">here</a> The dataset contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

### Preliminary Wrangling

1. The data was import using Pandas module and of the 81 variables, 12 variables were selected for analysis
2. 885 duplicates were found and they were all removed using drop_duplicates
3. The percentage of missinf values in each column were checked. since, the highest percentage of missing values was about 7%, each row containing missing values were dropped. After this, the dataset has 96896 rows and 12 variables

## Summary of Findings

> The majority of borrowers receive an APR of about 0.22 and the average debt to income ratio is about 0.25 which is 1:4. This implies that the income of most borrowers is times 4 of their debt.

> The distribution of monthly loan payment is right skewed with a mean of about 300. This shows that majority of the borrowers make a monthly loan payment that is less than 400. Also, the distribution of monthly income is skewed to the right too implying that few of the borrowers has a monthly income that is greater than 10000 while majority has an income of about 6000. It should be noted that most of the borrowers chose to hide their occupation by choosing Executive, Professional and Other, which does not really detail any occupation. Aside that, the most common occupations are computer programmer, teacher and analyst. The analysis also shows that having a source of income is important to secure a loan. It makes sense to give loan to people who are working except in rare cases. And owning a home does not really matter as there isn't much differences in thepercentage of those who do and doesn't.

> There is a negative correlation between the borrowers' APR and origination amount, monthly loan payment and stated monthly income. The higher these values, the smaller the APR. However, the monthly income of a borrower influences the amount of loan secured. The higher the monthly income, the higher the amount of loan secured. Also, the higher the original amount loaned, the longer the term but Monthly income does not affect the term of loan. It should be noted that owning a home slightly influences longer loan term. Overall, those who have a source of income take up loans for a longer period whereas those that are not employed or unavailable take up loans for a period of 3 years. No self-employed person took a loan of 1 year. And in all groups, majority take a loan of 3 years term

> Most of the borrowers with the highest origination amount of loan are judges, pharmacists and doctors while those with the least origination amount of loan are students, teacher's aides, waiters/waitresses and those who render food services. 

> The income range of 1-24,999 has a higher APR for homeowners than those who does not own a home.Starting at the 25,000 income range, APR is less for homeowners than their counterpart.

> There is no strong correlation among the numerical features, except the monthly loan payment and loan original amount that has a very strong positive correlation (0.93).

## Key Insights for Presentation

> The distribution of APR is unimodal at about 0.36 which means that majority of borrowers receive an APR of about 0.36. The average APR is about 0.22 while the distribution of loan origination amount is positively skewed and unimodal at about 3500 meaning that most of the borrowers took a loan that is below 10000 and most  collected a loan of about 3500. The average loan origination amount is about 8600. These two variables have a negative correlation. The higher the origination amount, the smaller the APR.

> One of the key factor that influences the original amount of loan is monthly income. The higher the income, the higher the loan amount. Those with a higher original amount of loan have a longer loan term. For instance, borrowers of a loan that is more than 10000 are likely to pay back in 5 years while those below 5000 mostly pay back within a year.