                          # Module 1: Introduction

# Module 2: Capital Investment Analysis
Capital budgeting: Decide how much to invest for future growth.\
A lot of analysis is involved to ensure the company is making good budgeting decisions \
Important to make good decisions for future growth

What happens in the decision making process?
1. Identify the project
  * Different types of investment projects. Can be:
  * Required investments (investments that improve things you’re required to provide/to comply with rules and regulations. Eg. delta airlines will invest in safety equipment = less liability/more efficient to make flights safer)
  * Replacement investments eg. have to replace old aircrafts, provide engineering services to other airlines?
  * Expansion investment (building bigger hangars?)
  * Diversification investment (should they invest in something that is not part of their main business) - rare to do this
  * Ideas for these projects come from: market research, find out what competitors are doing
2. Evaluate each project’s benefits and costs
  * Benefits: expected cash flow, how much cash will they gain from this
  * Discount rate = cost of capital
3. Selecting the project (what is the selection criteria for you to accept the project)
  * Metrics/rules used to select a project:
  * Net present value
  * Profitability index
  * Internal rate of return
  * Payback period
4. Implementation (what process are you going to follow for this project):
  * Monitor cash flows (is this cash flow what we are expecting)
  * Check that projects still meet the selection criteria
  * Do you still want to continue with the project or do you want to stop?

**Example: statement of cash flows from home depot**
|**Capex**: CAPital EXpenditure is cash flow from investing activities|
|---|

## Time Value of Money
* Before we start on understanding capital investment analysis, have to understand: Time Value of Money
* Same amount of money in the future is worth less than what you are receiving today.
* Opportunity cost of capital: rate of return sacrificed on the next best alternative
* Opportunity cost of 10%: investing now will give you a rate of return of 10%, do you still pick the 1000 now or 1500 in 5 years time.
* Opportunity cost of picking the 1500 in 5 years time is the amount of money you DON’T get from the 10% investment


### FUTURE VALUE:
How to compute future value? \
Money grows over time at rate r:

Future value of 1000 at rate=10% in 5 years is 1610

Future Value = Present Value * (1+r)^t \
R = interest rate, rate of return, opportunity cost of capital \
T = time (in years) \

Excel formula: FV()

### PRESENT VALUE:
More common method of evaluating your investment alternatives is to calculate the present value \
How much money would you need today in order to duplicate a future amount

Example with the 1500$ in 5 years time - what is the present value needed in order to reach that amount? (aka minimum present value needed to break even ish)

Just rearrange the formula: \
Present Value = Future Value / (1+r)^t

If you put the present value in the bank at the stated interest rate, you will reach 1500

If the calculated PV is lower than the other option (eg. PV of 1500$ is 930, other option for PV is 1000$)

Continue to pick the higher PV - this will result in an even higher FV

Excel formula: PV()

### Applications of Present Value and Future Value in capital investment

Basically just filling in the known variables and calculating for the unknown variables

There is also RATE() and NPER() functions in excel for return rate and number of periods

PMT (Payment): referring to what is the annual payment (eg. of a total lottery winning at a certain interest rate)

Also an excel function called PMT()


## Investment Selection Criteria

###Decision Rule #1: Net Present Value (NPV):
Forecasting the benefits and costs of the project for period T

What is T? \
Eg. if delta is buying an engine for 5 years use then T=5 \
Basically the how long the investment is expected to last \
Useful life of the project

(we are learning how to calculate cashflows in a later lesson. Right now, just assume that we already know the cashflows C1, C2 etc)

Usually C0 is negative because you invest a lot into a project at first

**Simple Rule:**
* NPV > 0 = accept project 
* NPV < 0 = reject project 
* NPV = 0 = go back and review your cashflow projections, can depend on other things

NPV is the most important value for shareholder value creation!!\
NPV will actualize as real cash 


**NPV Calculation Example:**\
So you can calculate NPV for each of these projects
For example project A: \
C0 = -100 \
C1 = 125 \
And \
R = 5%

Then plug it in to the NPV formula and calculate NPV

–

Different types of project: independent vs Mutually Exclusive Projects 
* Independent: accepting/rejecting the project is independent of accepting/rejecting the other projects. 
* Mutually Exclusive: if you accept this project A then you cannot accept project B (eg. you can only choose 1 manufacturer and not both)

If projects are **independent**: accept **all** because they all have positive NPV\
If projects are **mutually exclusive**: choose the one with the **highest NPV**



### Decision rule #2: Payback Period
How quickly can you recover the original investment made on the project?

The firm would already have decided what the payback cutoff period is. \
Any projects with a payback period greater than the cutoff will be rejected

If the projects are mutually exclusive, likely you will pick the project with the fastest payback period

But this isnt a great method to rely on for selecting a good investment project \
Payback period is arbitrarily decided \
Penalizes long term projects that may have very good investments in the long term but not in the short term \
Cashflows are completely ignored beyond the cut off period

Does not take into account time value of money

### Decision Rule #3: Internal rate of return
Looking at the discount rate (value of r) that makes the NPV of the project = 0

NPV approaches 0 as r increases \
(learning how to compute IRR in the next video)

Higher IRR is better \
If can pick all: choose those above a certain IRR \
If mutually exclusive: pick highest IRR 

Difficulties with using IRR:
* May have multiple IRR for the same project - curve is a parabola, 2 points where the curve intersects with the x-axis (x-axis is the IRR = you have 2 solutions for IRR)
* Can fail if u have a scale problem (projects are on different scales = not comparable using IRR)
  * Scale: the investment amount and timing for each projects are on different scales
  * 100% on $1 investment or 50% on $1000 investment? Scale of investment is different
* Can fail if u have a timing problem
  * Project A having a high return early but project B has a high return after a longer time period

Crossover rate: intersection of the curve

If 0<r<crossover rate, choose green line (higher NPV for that section) \
If crossover rate<r<infy, choose blue line (higher NPV for that section)

IRR can fail if the cost of capital is less than the crossover rate (sometimes cash flow can become negative the further right you go on the x-axis)

**Calculating crossover rate:** \
Can create a dummy project called project A-B => A cashflow - B cashflow for every time period => at some point you will get a time period where A-B = 0 (this is the crossover rate)

**TLDR IRR has a lot of problems**

### Decision rule #4: profitability index (benefit/cost ratio)
=> for every $ of investment how much are u getting

PI = (C0 + NPV) / C0

**Accept:** if PI > 1 (you get more than you are putting in)
**Or:** for mutually exclusive projects: use highest PI


### IRR vs NPV
How to compute cash flows

For independent projects: NPV and IRR will usually give the same results

**WHEN will IRR fail:**
* Non conventional cash flows (negative to positive or positive to negative, change in sign more than once)
* Mutually exclusive projects
* Projects where scale and timings differ

## Summary slide:
Apparently most real world companies prefer IRR and NPV

Some companies might use a higher cost of capital to select projects rather than the actual rate of return (eg. home depot’s actual r% might be 8% but they’ll say use 12% so u weed out the projects that barely breakeven)


## How to calculate cashflows for a capital investment project

Focus on how to estimate cash flows

Two key principles for estimating cashflows
Principle 1: record cashflow when the money actually moves and not when accounting using accrual concepts says they occur
Principle 2: imagine 2 worlds: one where the investment is made and one where the investment is rejected

Eg. marketing research cost is not included in investing cash flow


Microdyne:
Ad campaign costs 10M
If they do the ad campaign, their cash flow is 100k for the next 5 years
If they dont do the ad campaign, they lose 3M per year
Discount rate = 10%
Should they do the marketing campaign or not?

C0 = 10M

True benefit if they do the campaign = 3M + 100K (Incremental Principal)
(The gap between doing the campaign and not doing the campaign)
=> C1 to C5 = 3.1M

Now you have the cashflows => use the NPV function in excel to calculate the NPV



Costs that you will face in investment decision making:
Sunk Cost: Costs that you already spent and are not relevant for the present decision
Test Marketing Cost: Marketing research expenses expended
Erosion Cost: Cash flow transferred to a new project from sales, from old customers of other products of the firm (not everyone going to a new home depot store will be brand new, some are old customers who used to go to the old location)
Opportunity Cost: lost revenue from alternative uses of the investment. Next best alternative



Back to cash flows:
Depreciation: is a non-cash expense. Have to add depreciation back after tax.
After-tax Cash Flow (ATCF) 
= (Revenue - Costs - Depreciation)(1 - Tax) + Depreciation
= (Revenue - Costs)(1 - Tax) + Depreciation(Tax)


Working Capital:
Some amount of current assets will have to be locked up for the project (no longer current/liquid, now they are tied up in this investment)
Working capital at the start of the project: Treated as cash OUTFLOW
Working capital at the end of the project: Treated as cash INFLOW









Operating Margin = Revenues + Costs
Operating Cashflow = Operating Margin - Taxes
Capital Requirement = Capital Expenditure + Working Capital
Free Cashflow = Operating Cashflow - Capital Requirement
Cost of Capital = Cost of Debt + Cost of Equity
NPV = Free Cashflow - Cost of Capital


At the beginning of Week 1:
Role of the financial manager is to make good…
Investment decisions. For: increase CASHFLOW
Financing decisions. For: decrease COST OF CAPITAL
=> we can see:
=> NPV increases if CASHFLOW increases and COST OF CAPITAL decreases
=> role of financial manager ultimately is to increase NPV



Video Lesson 2: Example for calculating cashflows for a capital investment project
Example for cash flow calculator: Baffle Box
Last year: 
Machine: 11K
Economic life: 11y
Gross margin: 2K per year
Income before tax: 1K
Current Market Value: 5K (you can sell it off for 5K)
This year:
New machine for 15K
Economic life: 10y
Salvage value: 0
Gross margin: 4K per year
Income before tax: 2.5K
Depreciation: historical cost/useful life = 1500
Tax Rate: 45%
Cost of Capital after Tax: 10% (R%)

Q: Should the company replace the machine?
Recall: ATCF formula: 
After-tax Cash Flow (ATCF) 
= (Revenue - Costs - Depreciation)(1 - Tax) + Depreciation
Step 1: Calculate ACTF for both machines with the respective numbers
(we have no costs, tax is 0.45, depreciation is historical value/useful life)



Old Machine
New Machine
Gross
2000
4000
Minus Depreciation
-1000
-1500
Profit before tax
1000
2500
Tax (0.45)
-450
-1125
Profit after tax (1-0.45)
550
1315
Plus Depreciation
1000
1500
After Tax Cash Flow
1550
2875



Step 2: Incremental Principal for cashflow (C1 to Cn)
Calculate incremental benefits (Difference between NOT buying new machine vs buying new machine)
Don’t buy: ATCF = 1550
Buy: ATCF = 2875
Incremental benefit of buying the machine: 2875 - 1550 = 1325 for next 10 years

Step 3: Initial cash flow (C0)
= Outflow from selling the new machine (-15000) + inflow from selling the old machine (+5000)
= -10000

Step 4: Terminal Cashflow - what is terminal cashflow?
Cashflow at the end?
Anyway it’s 0

Step 5: Calculate NPV
We have everything needed to calculate NPV:
C0 = -10000 (Step 3)
C1 to C10 = 1325 (Step 2)
R% = 10% (Given in question as cost of capital after tax)

NPV 
= -10000 + 1325/(1.1) + 1325/(1.1^2) + …
= -1858

A: 
NPV IS NEGATIVE 
(NPV IS LESS THAN 1 = DO NO PROCEED WITH INVESTMENT PROJECT) 
= DO NOT REPLACE

(You may reconsider if you are able to find a buyer for the old machine for a higher price)



Video Lesson 3: Taking into account inflation when estimating cashflows for a capital investment project

Real vs Nominal Returns
Eg. you invest 1000 at 10%, but inflation is 5%:
Nominal returns: percentage change in the amount of money you have
Real return: percentage change in the amount of stuff you can actually buy


Fisher Effect:
(1 + Nominal Return Rate) = (1 + Real Return Rate)(1 + Inflation Rate)
APPROXIMATED: Nominal Return Rate = Real Return Rate + Inflation
Terms:
R = Nominal Return Rate
r = Real Return Rate
h = Inflation Rate



How does this apply in estimating cash flows:

Be consistent: express both cashflow and discount rate using the same return rate (whether real or nominal) - use nominal for both, or real for both - use fisher effect equation to move from one to the other

(Cost of capital is expressed in nominal terms, so it’s a good idea to forecast cashflows in nominal terms)

(Depreciation is always expressed in nominal terms)

Take into account inflation when dealing with:
Long horizons
High inflation rates



Sensitivity analysis:
You can do sensitivity analysis by asking ‘what-if’ questions:
Eg. what if the target market share is different? How does it affect NPV
Eg. What if COGS is more? Is it worthwhile doing?
Eg. What if inflation is more?
Eg. What if there’s a new competitor in 3 years? How will it affect your market share?
Eg. What if discount rate is higher?
Eg. What valuable options do you get from investing in the project?
You can address these questions by performing simulations with the “what if values”


Capital Investment Analysis Module Summary:
NPV is the most preferred technique
Calculating cashflows - done on incremental basis
Sunk costs are ignored
Opportunity costs and side effects must be considered
Correct handling of inflation - either apply inflation for both cashflow/discount rate, or don’t - be consistent
Uncertainty in forecasts can be addressed by conducting sensitivity analysis or simulations


List of all Excel Functions covered in Week 1:
FV()
PV()
RATE() - so the irritating thing about google sheets or this formula is that they automatically round to whole number instead of showing you the full thing for whatever reason (see: W1 self asseasment Q13)
NPER()
PMT()


Covered selection criteria for investment projects:
NPV
Payback Period
IRR
Profitability Index


Math formulas covered in Week 1:
Market Value of Equity - Lesson 2
Future Value - Lesson 4
Present Value - Lesson 4
Payment (PMT) - Lesson 5
Net Present Value (NPV) - Lesson 5
IRR - Lesson 7

Math formula covered: in week 2:
ATCF = (Revenue - Costs - Depreciation)(1 - Tax) + Depreciation (Lesson 1)

(1 + Nominal Return Rate) = (1 + Real Return Rate)(1 + Inflation Rate) 
APPROXIMATED: Nominal Return Rate = Real Return Rate + Inflation (Lesson 3)

r% = rate of return = cost of capital = discount rate = opportunity cost of capital


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

Enterprise Value: \
* EV = market value of equity + (market value of debt - cash) = market value of equity + net debt
* EV ratio = EV/EBITDA
* EBITDA is Earnings Before Interest/Taxes/Depreciation/Amortization
* EBITDA is a measure of total firm cashflow
* Market Value of Equity = Equity Value

### 3.1.8 Example Problems for Stock Valuation
#### Problem 1: FFDP Corp
* Revenue: $48M
* Expenses (Costs): $15M
* Debt: $64M
* Cash: $23M
* Number of Outstanding Shares: 1.95M
* EV/EBITDA Ratio: 6.4

Q1: What is the Enterprise Value (EV)? \
Q2: What is the stock price per share (P)?

A1: \
EBITDA = Revenue - Costs = 48M - 15M = 33M \
EV/EBITDA = 6.4 = EV/33M => EV = 6.4*33M = 211.2M

A2: \
EV = Market Value of Equity + debt - cash \
Market Value of Equity = EV - debt + cash = 211.2M - 64M + 23M = 170.2M \ 
Market Value of Equity is also = Stock Price * Number of outstanding shares => Stock Price = Market Value of Equity / Number of outstanding shares = 170.2M / 1.95M = 87.28

#### Problem 2: Storico Co.

# Module 4: Cost of Capital
# Module 5: Firm Valuation
# Module 6: Management for Value Creation
# Module 7: Summary
