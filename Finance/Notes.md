                          # Module 1: Introduction

# Module 2: Capital Investment Analysis

# Module 3: Stock Valuation
Previously: Creation of value using Capital Investment Analysis \
Current Module: Distribution of created value to stockholders 
## 3.0 Learning Objectives
1. Explain how stock prices depend on future dividends, and dividend growth
2. Compute stock prices using the Dividend Growth Model
3. Explain how growth opportunities affect stock values
4. Describe the PE (Price-Earnings) ratio
## 3.1 Valuation of Common Stock
The value of an asset is the present value of its expected **future cashflow**.
|**Future cashflow**: Refers to *future dividends* and *future capital gains*|
|---|

**Ways to estimate future cashflow:**
1. Zero Growth
2. Constant Growth
3. Differential Growth
### 3.1.1 Zero Growth
* Dividend does not grow over time => Dividend remains constant
* Dividend remains constant => Future cashflow remains constant
* A dividend that pays the same present value forever is called a **perpetuity**

|**Perpetuity**: Refers to an asset that pays a stated return for an infinite time.|
|---|

Equation: 

$`P_0 = P_1 = P_2 = ... =\frac{Div_{t=1}}{(1+R)^1} + \frac{Div_{t=2}}{(1+R)^2} + \frac{Div_{t=3}}{(1+R)^3} + ... + \frac{Div_{t=\infty}}{(1+R)^\infty} = \frac{Div}{R}`$ 

Where $`P_0`$ is the price of the stock at time $`t=0`$. 

**Note**: No indication for which time period $`Div`$ is in (eg. $`Div_0`$ or $`Div_1`$) because they are ALL THE SAME.

Therefore, in a zero growth model, the stock valuation is simply the present value of all future cashflows.

This is the constant dividend divided by the cost of capital.

### 3.1.2 Constant Growth
* Dividend grows at a constant growth rate $`g`$
* Dividend grows at a constant rate = Future cashflow grows at a constant rate
* A dividend that grows at a constant rate forever is called a **growing perpetuity**

**Equation:** 

$`Div_{t=1} = Div_{t=0}(1+g)`$ 

$`Div_{t=2} = Div_{t=1}(1+g) = Div_{t=0}(1+g)^2`$ 

$`Div_{t=3} = Div_{t=2}(1+g) = Div_{t=0}(1+g)^3`$ 

$`...`$ 

$`Div_{t=n} = Div_{t=n-1}(1+g) = Div_{t=0}(1+g)^n`$ 


**This reduces to:** 

$`P_n = \frac{Div_{n+1}}{R-g} `$

**Note:** The numerator of this formula is $`Div_1`$ and NOT $`Div_0`$.
**Note:** This formula calculates the CURRENT ($`t=0`$) perpetuity using the NEXT ($`t=1`$) period's dividend.

**Constant Growth Example** 
Price of a dividend that was just paid out = $`Div_0`$ = $0.50 \
Growth of dividend per year = $`g`$ = 2% \
Return on capital = $`R`$ = 15% \

Hence selling price of the stock: 

$`P_0 = \frac{Div_0(1+g)}{R-g} = \frac{0.50 \times (1+0.02)}{0.15 - 0.02}`$ = $3.92

### 3.1.3 Differential Growth
* Dividend grows at one rate in the beginning and then a different constant rate after some time.

**Differential Growth Example** 

Price of a dividend that was just paid out = $`Div_0`$ = $2 \
Initial growth rate = $`g_1`$ = 8% for 3 years \
Perpetuity growth rate = $`g_2`$ = 4% after 3 years till forever \
Return on capital = 12%

From 0-3 years:  

Year 1: $`Div_1 = Div_0(1+g_1)^1 = 2(1.08)^1 = 2.16`$ \
Year 2: $`Div_2 = Div_0(1+g_1)^2 = 2(1.08)^2 = 2.33`$ \
Year 3: $`Div_3 = Div_0(1+g_1)^3 = 2(1.08)^3 = 2.52`$ 

From year 4 onwards: 

Year 4: $`Div_4 = Div_0(1+g_1)^3(g_2)`$

Constant growth phase beginning in year 4 can be valued as a growing perpetuity at year 3: 

$`P_{t=3} = \frac{Div_4}{R-g_2} = \frac{2\times1.08^3\times1.04}{0.12-0.04} = 32.75`$

Hence selling price of the stock: 

$`P_0 = \frac{Div_1}{(1+R)^1} + \frac{Div_2}{(R+1)^2} + \frac{Div_3 + P_3}{(R+1)^3} = \frac{2.16}{(1.12)} + \frac{2.33}{(1.12)^2} + \frac{2.52 + 32.75}{(1.12)^3}`$ = $28.89

Generalised formula:

$`P_0 = \frac{Div_1}{(1+R)^1} + \frac{Div_2}{(1+R)^2} + ... + \frac{Div_n + P_n}{(1+R)^n}`$ 

Where $`n`$ is the number of years 'in the beginning'.

### 3.1.4 Estimation of Parameters
* Value of firm depends on growth rate $`g`$ and discount rate $`R`$.

**Estimationg of growth rate $`g`$**

$`g`$ = Retention Ratio $`\times`$ Return on Equity \
= (1 - Dividend per share) $`\times`$ Return on Equity \
= (1 - Dividend per share) $`\times`$ (Net Income $`\div`$ Avg Equity)

**Estimating discount rate $`R`$**

$`P_0 = \frac{Div_1}{R-g} \implies R = \frac{Div_1}{P_0} - g`$

**Note:** In reality, there is a lot of error in estimating R. \
Good idea to do sensitivity analysis for estimation of R.

### 3.1.5 Growth Opportunities
* A company's stock price can be broken up into 2 portions:
  1. Part 1: Dividends
  2. Part 2: Net Present Value of Growth Opportunities

P = (Earnings per Share $`\div`$ R) + NPV of Growth Opportunities

**Case where company is not growing:** 
* NPV of Growth Opportunities = 0 
* Hence, P(Not Growing) = (Earnings per Share $`\div`$ R) + 0

These kinds of companies are called **cash cows**.

**Case where company is growing:**
* NPV of Growth Opportunities > 0 
* Hence, P(Growing) = (Earnings per Share $`\div`$ R) + NPV of Growth Opportunities 
* And P(Growing) > P(Not Growing)

**Example Calculation for Growth Opportunities**
EPS = $5 \
Discount rate = R = 16% \ 
Price of share = P = $75 

$`P = \frac{EPS}{R} + NPVGO \implies 75 = \frac{5}{0.16} + NPVGO`$

$`NPVGO = 75 - \frac{5}{0.16} = 43.75`$

### 3.1.6 Retention Rate and Firm Value
* Increase in retention rate = increase in firm's growth rate = increase in value of firm = decreases dividends
* 

### 3.1.7 Price-Earnings Ratio
* Current stock price divided by annual EPS
* P/E ratio = price per share / earnings per share
* P/E ratio is positively related to growth opportunities

Recall: \
P = (EPS/R) + NPVGO \
=> divide everything by EPS \
=> 1/EPS * P = 1/EPS * (EPS/R + NPVGO) \
=> P/E = 1/R + NPVGO/EPS

2 firms can have the same EPS but different share prices => this is because the 2 firms are growing at different rates

Enterprise Value Ratio: \
* EV = market value of equity + (market value of debt - cash) = market value of equity + net debt
* EV ratio = EV/EBITDA
* EBITDA is Earnings Before Interest/Taxes/Depreciation/Amortization
* EBITDA is a measure of total firm cashflow

### 3.1.8 Example Problems for Stock Valuation

# Module 4: Cost of Capital
# Module 5: Firm Valuation
# Module 6: Management for Value Creation
# Module 7: Summary
