The data set we choose is **Loan Data from Prosper**.

# Exploratory Data
## Univariate Exploration

Main variable of interest:
 - LoanStatus(loan’s outcome)
 - BorrowerAPR
 - BorrowerRate

We compared then with other main variable and explore their relationship.

### LoanStatus

LoanStatus is a categorical variable.
The most loan status are **completed** and **current**. About 50% of loan status are current.


### BorrowerAPR

BorrowerAPR is a numerical variable.
The mean of borrowerAPR be 0.218827655909788. Here is a high density around 0.36.


### BorrowerRate

BorrowerRate is a numerical variable.
The mean of borrower rate be 0.1927640577687518. Here is a high density around 0.3.


### BorrowerState

BorrowerState is a categorical variable.
The most loan borrower state is **CA**, about 1/8 of the total amount. Then is TX, NY, Fl.

### Occupation

Occupation does not provided many useful information.

### EmploymentStatus

EmploymentStatus is a categorical variable.
The most employment status is **employed**, then is **full-time**. More than 50% are employed, about 45% are full-time.


### Employment status duration

Employment status duration is a numerical variable.
Employment status duration has a right-skewed distribution. With a mean of 96.07158175934984.


### DebtToIncomeRatio

Debt to income ratio is a numerical variable.
Debt to income ratio has a highly right-skewed distribution. With a mean of 0.2759466040063403.


### StatedMonthlyIncome

Stated monthly income is a right-skewed distribution.

### MonthlyLoanPayment

Monthly loan payment is a right-skewed distribution.

### Investors

Investors is a right-skewed distribution.



## Bivariate Exploration

### LoanStatus vs BorrowerState

The state have more loan are **CA**, **FL**, **IL**, **NY** and **TX**.
All of them have more current loan, then completed loan.

This is same as our discovery in LoanStatus and BorrowerState.
Completed CA loan amount is larger than other current loan in other state.
Beside that we can not see clear relationship between these two.


### LoanStatus vs BorrowerAPR

**Completed** loan status has lowest borrowerAPR. **PastDue(91-120 days)** has the highest borrowerAPR.
If we group past due together, past due still has the highest borrowerAPR.
Completed loan status has the largest range of borrowerAPR. Canceled loan status has the narrowest range of borrowerAPR.


### LoanStatus vs BorrowerRate

**Completed** loan status has lowest borrower rate. **PastDue(91-120 days)** has the highest borrower rate, which is same as borrower rate.
If we group past due together, past due still has the highest borrower rate.
Defaulted loan status has the largest range of highest borrower rate. Canceled loan status has the narrowest range of borrower rate.


### LoanStatus vs EmploymentStatus

The largest amount of loan are belongs to **current+employed**.
Then is **full-time+completed**, **completed+employed**.


## LoanStatus vs EmploymentStatusDuration

**Current load status** has the largest employment status duration, **cancelled** has the lowest employment status duration.


## LoanStatus vs DebtToIncomeRatio**

**Cancelled** load status has the lowest debt to income ratio and **past due(16-30 days)** has the largest debt to income ratio.
If we group past due together, **past due** still has the largest debt to income ratio.


## LoanStatus vs MonthlyLoanPayment

**Cancelled** load status has the lowest monthly loan payment and **current** has the largest monthly loan payment.


## LoanStatus vs Investors

**Current** load status has fewest investors and **completed** load status has most investors.


## BorrowerAPR vs BorrowerState

The higher Borrower APR are from AR and AL and MS.
The lower Borrower APR are from ME and IA.

Among smaller BorrowerAPR  and larger BorrowerAPR, the highest and lowest states are different.
Among the larger Borrower APR, the highest is LA, lowest is ME.
Among the smaller Borrower APR, the highest is SD, lowest is VT.


## BorrowerAPR vs EmploymentStatus

The higher Borrower APR are from not employed.
The lower Borrower APR are from part-time.

Among the larger Borrower APR, the highest is not employed, lowest is unknown(not available).
Among the smaller Borrower APR, the highest is other status, lowest is full-time.

## BorrowerAPR vs EmploymentStatusDuration

There is a not clear obvious normal distribution between borrower APR and employment status duration.

We see no clear relationship between:
 - BorrowerAPR vs DebtToIncomeRatio
 - BorrowerAPR vs StatedMonthlyIncome
 - BorrowerAPR vs MonthlyLoanPayment
 - BorrowerAPR vs Investors

## BorrowerRate vs BorrowerState

In general, MD, MO, AL have higher borrower rate.
IA, ME have lower borrower rate.

MD, SD, ND have higher borrower rate among lower borrower rate.
AL, OR have lower borrower rate among lower borrower rate.

ND has higher borrower rate among higher borrower rate.
IA has lower borrower rate among lower borrower rate.


## BorrowerRate vs Investors

There is a right skewed relationship between BorrowerRate and investors.


# Multivariate Exploration

## LoanStatus vs BorrowerState vs BorrowerAPR

The higher Borrower APR are from AR and AL.
AR has a higher borrower AR in defaulted load status.
AR and AL have a higher borrower AR in past due load status.

The lower Borrower APR are from ME and IA.
ME and IA in all load status are having a load borrower APR.

Amoung the smaller Borrower APR, the highest is SD. And SD have a high borrower APR in defaulted and past due load status.


## LoanStatus vs EmploymentStatus vs BorrowerAPR

Employed people are having a higher borrowerAPR than others in defaulted load status.
Self employed people are having a higher borrowerAPR than others in final payment progress.
Not employed people are having a high borrower APR in current and past due load status.
