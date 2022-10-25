# Data-Visualization-Project

## Dataset
**Loan Data from Prosper** 
This dataset contains 113,937 loans with 81 variables on each loan and can be found [here](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&amp;sa=D&amp;ust=1581581520570000)

For this analyses, only 15 variables have been used. These include `ListingKey`, `ListingCreationDate`, `CreditGrade`,`Term`,`LoanStatus`,`BorrowerAPR`,`ProsperRating (Alpha)`, `ListingCategory (numeric)`,`EmploymentStatus`,`IsBorrowerHomeowner`,`CreditScoreRangeLower`, `CreditScoreRangeUpper`,`IncomeRange`, `StatedMonthlyIncome`,`LoanOriginalAmount`,`MonthlyLoanPayment`]. A description of these variables is found in the [data dictionary](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0)

## Data Wrangling
The forementioned variables were selected for expolartion and the rest dropped. The `listingcreationdate` was converted to the correct data type and the variable `year` from corresponding birth_date column value. I also created the `meancreditrating` variable by getting the average between the upper and Lower credit rating. Further, i created the `ListingCategory` variable by replacing the numeric entries with the actual listing entry. 

Univariate, bivariate and multivariate plots have been used to communicate data findings.
## Summary of Findings

* From the data, we can see that majority loans were issued after 2009. the latter had the least amount of loans issued, the number increased steadily peaking at 2013.
* The distribution of loan amounts is skewed to the right. there are peaks at $5000, $10000, $15000, $ 20000 and $25000. **This has been adopted in the presentation**
* The borrowerAPR is normally distributed. using smaller bins shows a peak at around 0.36
* We can see that most of the loans had a term of 36 months. only a few had a term of 12 months
* Majority of the Loan borrowers ,approximately 60%, were employed
* majority of the loan borrowers falls under the income range of 25,000-49,999 closely followed by those in the range 50,000-74,999.
* Majority of the borrowers listed Debt consolidations the reason for borrowing, we can note that most of the borrowers did not indicate the reason for borrowing while the third, fourth and fifth reasonsfor borrowing were other, home improvement and business respectively.
* The mean credit score is skewed to the right with the peak score at around 700. the seems to be outliers with a mean credit score of 9.5. for those who listed Not applicable for employment status
* Majority of the loans are current (49.66%) while 33.42% are completed. However, 10.53% & and 4.4% of the loans have been charged off and defaulted respectively.
* There is a negative correlation between BorrowerAPR & Mean credit Rating. AS the Mean credit Rating increases, the  BorrowerAPR  decreases
* There is a negative correlation between BorrowerAPR & Loan Original Amount. Higher loan amounts have a lowere interest rate
* There is a positive correlation between mean credit score and loan original amount. borrowers with a higher mean credit score have relatively higher loan amounts. **This has been adopted in the presentation**
* From the first income range of 1-24999, the loan amounts increases steadily up to the top range of 100000. Those within the 100000 income range had the highest LoanOrignationamount. suprisingly, borrowers with an income of 0 had relatively higher loan amounts compared to those in the range 1-24999.
* Generally, those stated being in full time and part time employment had a relatively low interest rates on their loans as compared to those stated that they were unemployed. **This has been adopted in the presentation**
* More borrowers in the lower income bands ( 0,1−24,999, 25,000-49,999) and those who we not employed or did not display the income did not own homes. On the other hand, more borrowers in the higher income bands ( 50,000−74,999, 75,000-99,999, $100,000+) reported owning homes.
* Non-home owners had higher loan interest rates compared to homeowners
* Home owners were more likely to have a higher credit score and higher loan original amount compared to non home owners
* Generally, home owners had relatively low interest rates compared to non homeowners across all employments levels except those that stated that they were not employed. for the latter, home owners had a relatively higher interest rates compared to none home owners.
