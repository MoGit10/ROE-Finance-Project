# Revenue Growth, Profitability, and Stock Performance Among Major U.S. Banks

## The Question

My thought when starting this project was simple:

**Companies that are more profitable should produce better returns for investors.**

It sounds reasonable. If a company is making more money from its resources and shareholders' capital, shouldn't its stock perform better?

To test that idea, I analyzed five of the largest U.S. banks:

- JPMorgan Chase (JPM)
- Bank of America (BAC)
- Wells Fargo (WFC)
- Goldman Sachs (GS)
- Morgan Stanley (MS)

Using Python and the Yahoo Finance API, I collected financial statement data and historical stock prices for each company.

My goal was straightforward: **determine whether profitability or revenue growth better explains stock performance.**

---

## Step 1: Measuring Profitability

The first metric I analyzed was **Return on Equity (ROE)**, one of the most common measures of profitability.

ROE shows how efficiently a company generates profit from shareholders' equity. A higher ROE generally means a company is making better use of the money invested by its shareholders.

After calculating ROE for each bank, I found the following:

| Company | Return on Equity (ROE) |
|---------|------------------------:|
| JPM | 15.74% |
| MS | 15.10% |
| GS | 13.74% |
| WFC | 11.78% |
| BAC | 10.06% |

From this first analysis, **JPMorgan** appeared to be the strongest performer. That wasn't too surprising, considering JPMorgan is widely viewed as the powerhouse of Wall Street under Jamie Dimon's leadership.

If my original hypothesis was correct, JPMorgan should also have produced the highest stock return.

---

## Step 2: Looking at Stock Returns

Next, I calculated each company's one-year stock return.

The results were much different than I expected.

| Company | One-Year Stock Return |
|---------|----------------------:|
| GS | 83.96% |
| MS | 71.14% |
| BAC | 24.80% |
| JPM | 20.99% |
| WFC | 11.36% |

Goldman Sachs and Morgan Stanley significantly outperformed the rest of the group.

Meanwhile, JPMorgan, despite having the highest ROE, delivered a much smaller return.

At this point, my original idea didn't seem to hold up. Profitability alone wasn't explaining stock performance.

So I wanted to measure the relationship more formally.

---

## Step 3: Testing the Relationship

To see whether ROE was actually related to stock performance, I calculated the correlation between the two.

The correlation came out to:

**ROE vs. Stock Return = 0.396**

A positive correlation means companies with higher ROE tended to have higher stock returns, but **0.396 is only a moderate relationship**.

In other words, profitability explained **some** of the variation in stock performance, but not nearly enough to support my original hypothesis.

That led me to another question:

**Maybe investors care more about growth than profitability.**

---

## Step 4: Looking at Revenue Growth

Next, I calculated each bank's annual revenue growth.

| Company | Revenue Growth |
|---------|---------------:|
| MS | 14.48% |
| GS | 8.92% |
| JPM | 7.32% |
| BAC | 6.84% |
| WFC | 1.70% |

Unlike ROE, these rankings looked much closer to what I saw in the stock returns.

Morgan Stanley and Goldman Sachs were near the top in both revenue growth and stock performance.

That suggested revenue growth might be a better indicator of future stock returns.

---

## Step 5: Comparing Revenue Growth to Stock Returns

I then calculated the correlation between revenue growth and one-year stock returns.

The result was:

**Revenue Growth vs. Stock Return = 0.757**

This was a much stronger relationship than the one I found using ROE.

While this doesn't prove that revenue growth causes higher stock returns, it does suggest that investors may place greater value on companies that are growing their business rather than simply generating high profits today.

---

## What I Learned

When I started this project, I expected profitability to be the strongest driver of stock performance.

Instead, the data pointed me in a different direction.

Among these five major banks, **revenue growth had a much stronger relationship with stock returns than Return on Equity.**

This project was also a good reminder that assumptions should always be tested with data. Even when an idea sounds logical, the numbers can tell a different story.

---

## Tools Used

- Python
- Pandas
- Matplotlib
- Yahoo Finance (yfinance)
- Google Colab

---

## Skills Demonstrated

- Financial Statement Analysis
- Financial Markets Research
- Data Collection
- Data Cleaning
- Python Programming
- Data Visualization
- Correlation Analysis
