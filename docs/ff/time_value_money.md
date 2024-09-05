# Time Value of Money
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


