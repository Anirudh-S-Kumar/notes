The main idea is that a dollar today is worth more than a dollar tomorrow. This is because you can invest that dollar today and have more than a dollar tomorrow. This is the concept of the time value of money. This has the following affects

- *Spending* - You can buy more with 1000 Rs today than 1000 Rs a year from now.
- *Investing* - You can invest 1000 Rs today and have more than 1000 Rs a year from now.
- *Borrowing* - You borrow money today and pay back more than you borrowed.

Reasons for the time value of money are:

- *Inflation* - The value of money decreases over time.
- *Uncertainty* - Money today is more certain than money tomorrow.

## Compounding

$$FV = PV(1 + i)^{n * t}$$

Where:

- $FV$ = Future Value
- $PV$ = Present Value (Principal): The larger the principal, the greater the returns.
- $i$ = Interest Rate: The higher the interest rate, the greater the returns.
- $n$ = Number of compounding periods per year: The more compounding periods, the greater the returns.
- $t$ = Number of years: The longer the time, the greater the returns.

### Continuously Compounded Interest

$$FV = PV  e^{i * t}$$

### Interest Factor

$$FVIF = (1 + i)^t$$

$$PVIF = \frac{1}{(1 + i)^t}$$

!!! note
    - Rule of 72: To find out how long it takes to double your money, divide 72 by the interest rate.

??? Question

    1, How much amount will one have in 30 hears if one invests Rs. 10,000 @ 10% p.a.

    - Simple interest: $FV = 10000 * (1 + 0.1 * 30) = 40000$
    - Compounded annually: $FV = 10000 * (1 + 0.1)^{30} = 174494.02$
    - Compounded Continuously: $FV = 10000 * e^{0.1 * 30} = 200855$

## Timeline of Cash Flows
- 1000 Rs Lumpsum in 2 years
    ```mermaid
    timeline
        0   :   
        1   :  
        2   : 1000
    ```
- 3-year Rs 100 ordinary annuity
    ```mermaid
    timeline
        0   : 100
        1   : 100
        2   : 100
        3   : 100
    ```
- Uneven cash flow stream
    ```mermaid
    timeline
        0   : -50
        1   : 100
        2   : 75
        3   : 50   
    ```

??? Question "What is the future value of an initial Rs. 100 after 3 years if the interest rate is 10%?"

    Finding FV of cash flow is called ==compounding==

    - After 1 year: $FV = 100 * (1 + 0.1) = 110$
    - After 2 years: $FV = 110 * (1 + 0.1) = 121$
    - After 3 years: $FV = 121 * (1 + 0.1) = 133.1$

??? Question "Present Value of Rs. 100 due in 3 years at 10%?"
    Finding PV of cash flow is called ==discounting==

    - After 1 year: $PV = \frac{100}{1 + 0.1} = 90.91$
    - After 2 years: $PV = \frac{100}{(1 + 0.1)^2} = 82.64$
    - After 3 years: $PV = \frac{100}{(1 + 0.1)^3} = 75.13$

??? Question "5% compounded semi-annually, or 10% compounded annually, which is better?"

    - 5% semi-annually: $FV = 100 * (1 + 0.05)^{2 * 3} = 134.01$
    - 10% annually: $FV = 100 * (1 + 0.1)^3 = 133.1$

    5% semi-annually is better.

## Annuities

Annuities are a series of equal payments made at regular intervals. 
### Future Value of Annuity

$$FVIFA = A + A(1 + r) + A(1 + r)^2 + \ldots + A(1 + r)^{n - 1} = A \frac{(1 + r)^n - 1}{r}$$

FVIFA - **F**uture **V**alue **I**nterest **F**actor of **A**nnuity

??? question "Future Value of $1000 invested at 5% for 5 years?"
    $FVIFA = 1000 \frac{(1 + 0.05)^5 - 1}{0.05} = 1276.28$

### Present Value of Annuity

$$PVIFA = \frac{C}{(1 + r)} + \frac{C}{(1 + r)^2} + \ldots + \frac{C}{(1 + r)^n} = C \frac{1 - (1 + r)^{-n}}{r}$$

There are two types of annuities:

- **Ordinary Annuity**: Payments are made at the end of the period.
- **Annuity Due**: Payments are made at the beginning of the period.

$$PVIFA_{\text{Ordinary}} = \frac{C}{(1 + r)} + \frac{C}{(1 + r)^2} + \ldots + \frac{C}{(1 + r)^n} = C \frac{1 - (1 + r)^{-n}}{r}$$

$$PVIFA_{\text{Due}} = C + \frac{C}{(1 + r)} + \ldots + \frac{C}{(1 + r)^{n - 1}} = C \frac{1 - (1 + r)^{-n}}{r} (1 + r)$$


## Perpetuities

Perpetuities are annuities that continue indefinitely.

$$PV= \frac{C}{r}$$

### Growing Perpetuities

Perpetuities that grow at a constant rate, say $g$.

$$PV = \frac{C}{r - g}$$

For a growing fixed maturity annuity:

$$PV = \frac{C}{1+r} + \frac{C(1+g)}{(1+r)^2} + \ldots + \frac{C(1+g)^{n-1}}{(1+r)^n} = \frac{C}{r-g}\left(1-\frac{(1+g)^n}{(1+r)^n}\right)$$


## Loan Amortization

Loan amortization is the process of paying off a loan in installments. Let's construct an amortization schedule for a loan of Rs. 1000 at 10% p.a. with 3 equal payments.

1. Find the required annual amount
    - $$ 1000 = A * PVIFA_{\text{Ordinary}} = A \frac{1 - (1 + 0.1)^{-3}}{0.1} = A * 2.4869$$

    $$ A = 1000 / 2.4869 = 402.11$$

    !!! note 
        Remember that $FV = 0$ as the reason for amortization is to pay off the loan.

1. Find interest paid in first year
    - $I_1 = 1000 * 0.1 = 100$
1. Find principal repaid in first year
    - $P_1 = A - I_1 = 402.11 - 100 = 302.11$
1. Find outstanding balance after first year
    - $B_1 = 1000 - P_1 = 1000 - 302.11 = 697.89$
  
| Year | Beginning Balance | Payment | Interest | Principal | Ending Balance |
|------|-------------------|---------|----------|-----------|----------------|
| 1    | 1000              | 402.11  | 100      | 302.11    | 697.89         |
| 2    | 697.89            | 402.11  | 69.79    | 332.32    | 366            |
| 3    | 366               | 402.11  | 36.6     | 365.51    | 0              |

- Total interest paid = 100 + 69.79 + 36.6 = 206.39
- Total payment = 402.11 * 3 = 1206.33

