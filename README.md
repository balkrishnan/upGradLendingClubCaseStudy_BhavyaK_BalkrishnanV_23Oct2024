## LendingClubCase_upGrad_BhavyaKapoor_BalkrishnanVenkiteswaran
========================================================================
# Lending Club Case Study


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Proposals to Lending Club's Management Team](#proposals)
* [Acknowledgements](#acknowledgements)

## General Information
- Provide general information about your project here.
  >> We are analyzing a loan-dataset to identify the patterns from past-history of loan disbursement, so that it would indirectly help the lending company determine if the loans to an applicant should be approved or not.
- What is the background of your project?
  >> You work for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company
The data given below contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.
In this case study, you will use EDA to understand how consumer attributes and loan attributes influence the tendency of default.
  >> When a person applies for a loan, there are two types of decisions that could be taken by the company:
Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:
Fully paid: Applicant has fully paid the loan (the principal and the interest rate)
Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.
Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 
Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)
- What is the business probem that your project is trying to solve?
  >>Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the LC when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the LC Management. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 
If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.
In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment. 
- What is the dataset that is being used?
  >> 'loan' dataset contains the complete loan data for all loans issued through the time period 2007 t0 2011.

## Libraries Used
- Pandas
- Seaborn
- Matplotlib

## Proposals to Lending Club's Management Team
>> The strong correlation between pub_rec and pub_rec_bankruptcies implies that bankruptcy is a significant factor in public records. More attention should be given to customers with a history of public records or bankruptcies when evaluating loan risk.

>> Moderate correlations between DTI, revolving balances, and revolving utilization suggest borrowers should manage their overall debt load and credit utilization better to avoid high-interest rates.

>> Higher revolving balances increase revolving utilization, which can affect the borrower’s credit score and loan approval chances. LC could offer proactive tools like alerts for high revolving balances or recommend setting up automatic payments to maintain utilization below 30% for optimal credit health.

>> Borrowers with high credit utilization tend to face higher interest rates. LC Management could encourage these borrowers to lower their utilization by offering credit line reductions, balance transfer options, or lower interest rates for accounts with reduced utilization, helping reduce the overall risk.

>> LC management must review their policies on why Grade ‘B’ and ‘C’ loans are mostly defaulted.

>> LC management must review their policies on why these three sub-grade loans, ‘B3’, ‘B4’ and ‘B5’, are mostly defaulted.

>> LC management must verify the financial and vocation credentials of borrowers, especially where higher Installment-Amounts are involved, the feasibility of repayment of installments consistently. 

>> LC management must verify the financial and vocation credentials of borrowers, especially where higher Interest-Rates are involved, the feasibility of repayment of installments.  

>> LC management can offer more loans in medium-interest-rate category due to their popularity and for also positive-closures resulting in profits to LC.  

>> LC management can offer more variety of loans of 36-month period due to higher closure-rate and popularity. This will help increase the profits of LC. 

>> LC management can limit the Loan-Amount values to increase the possibility of FULLY-PAID category. This will help the LC minimize their losses. 

>> LC management must ensure that due-diligence on the borrowers are done based on their Annual-Income to minimize defaults. 

>> LC management could focus on borrowers who are in their first job and make it attractive for them to take loans. This helps LC increase their lending.

## Acknowledgements
- This project was proposed by [upgrad.com](https://learn.upgrad.com/course/5810/segment/54646/325499/985632/4924761).

## Contact
Created by [bhavyarocks19@gmail.com],[balkrishnan.venkiteswaran@gmail.com] - feel free to contact us!


## License
This project is open source and available under the [MIT License](https://github.com/balkrishnan/upGradLendingClubCaseStudy_BhavyaK_BalkrishnanV_23Oct2024/blob/main/LICENSE).
