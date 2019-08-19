---
title: Investigating Seasonality
image: /assets/img/blog/seasonalitybg.jpg
description: >
  Does seasonality really exists and profitable?
---

There are many interesting seasonal patterns where you can use on your investment decisions. Although there are only a few people talk about this. 

These seasonal effects are well-known and said profitable on most types of markets.
Announcement Days is one of the popular seasonal events where everyone is waiting for as it can push huge pumps for positive stories or a negative swing. I wonder if we can make money by determining when to trade based on repeating events that are moved by economic factors and find evidence of this. Is this how easy trading based on seasonality? Does this mean that we are printing money on these repeating events? Is this a billion-dollar strategy with the secret edge? Oh maybe you can “Sell in May, Go Away!” thing since someone told me that stocks are historically underperforming from May to October? Don’t get too excited. Always remember that

> Markets are super efficient and a lot of madness going on. Embrace the Uncertainty
{:.lead}

The main point of this article is to investigate some of the well known seasonal pattern using historical and economic data we will uncover useful insights from the analysis and decide whether it helps us on our investment decisions. So we’re going to need some tools for investigating seasonality effects in financialassets. Something a bit cruder, and a bit more flexible, given the massive amounts of noise in our data. The data is already prepared for us to look into these patterns and I chose BDO and SM as our subject of interest.

Before that, It's always smart to review what other people have found.


### The January Effect
Momentum tends to outperform in December and under-perform in January
There is some evidence that January returns are somewhat predictive of the full year returns.

**PAPER**: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1166149
{:.message}

Okay, so now at least some people observe this effect and it's up to us to investigate the evidence of its existence. To start our analysis I have prepared the data of BDO stock from 2002-2019 (August) then use excel to plot the return values.

Lets take a quick look on monthly return if we just go Long position on the whole year.

![Full-width image](/assets/img/blog/seasonality/monthly-returns.png){:.lead data-width="800" data-height="100"}

Hmmm ... December has the highest return from 2002 - 2018, Interestingly January has weak returns. Is this what we are looking for? Let us compare December and January again side by side to have a clearer outlook.

![Full-width image](/assets/img/blog/seasonality/dec-jan-returns.png){:.lead data-width="800" data-height="100"}

It looks random now, we cannot guarantee a seasonal pattern here, it may be profitable from 2008-2012 but the following years did the effect lost its edge? what the heck happened last 2013? Is it because of typhoon Yolanda on November that wrecks most BDO office then recovered on January?   

This is why we have to embrace the uncertainty, in the market we cannot guarantee the future due to its madness we can only estimate from the sea of noise and we are going to look for it back up with data and evidence. It is wise to do in-depth research of the market before throwing your money into your broker.

Alright, let's go back and see the last piece of the puzzle that we are trying to look for in the January Effect. We are going to check whether the returns are stable across different years, We have only looked into 2 charts from 2002-2019 and that's not enough to make a wrap-up.

2012-2016
![Full-width image](/assets/img/blog/seasonality/2012-2016.png){:.lead data-width="800" data-height="100"}

2013-2017
![Full-width image](/assets/img/blog/seasonality/2013-2017.png){:.lead data-width="800" data-height="100"}

2014-2018
![Full-width image](/assets/img/blog/seasonality/2014-2018.png){:.lead data-width="800" data-height="100"}

I don't think there's a seasonal January effect on BDO. Do you think that it would exist on other tickers? and market like currencies? Who knows maybe I am just unlucky in selecting which asset to analyze.

Before we move on to the next seasonal effect, this is the running total return in years if we go Long from 2012-2019


![Full-width image](/assets/img/blog/seasonality/january-effect.png){:.lead data-width="800" data-height="100"}

I'll leave to you interpreting the chart, is it safe to invest in December? Is the effect changing regime? this might be no brainer to others because of the holidays.  

### Halloween
Average stock market returns have been higher between November and April and low between May and October.

This is the “Sell in May and Go Away” trade!

**PAPER**: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=300700
{:.message}

Okay, let's inspect additional stock for this effect. First, we are going to take a quick look into SM monthly returns for 2005-2019

![Full-width image](/assets/img/blog/seasonality/sm-monthly-returns.png){:.lead data-width="800" data-height="100"}


How about in BDO?

![Full-width image](/assets/img/blog/seasonality/monthly-returns.png){:.lead data-width="800" data-height="100"}

We should expect that the returns are higher between November and April and low between May and October. Did you observe a Halloween effect based on the two charts?
let's combine both tickers and plot them to make it neat

![Full-width image](/assets/img/blog/seasonality/smbdo-monthly-returns.png){:.lead data-width="800" data-height="100"}



Hmm ... its kinda random, and it might be true to SM but not on BDO but if you look carefully there's a higher return on SM on September and May for BDO, did this invalidate the Halloween effect? or are those months outlier? is there something special that we are not aware of specifically on those stocks? This is how to market madness in reality works, we cannot guarantee patterns the market will always move automagically without knowing the causes all we can do is embrace it and decide rationally. Since we only inspected two stocks we aren't able to draw a good conclusion about this hypothesis, if you have the luxury of time to do analysis on more than what we explored feel free to share it to the community.

Since we talked about Halloween why not Ghost month? a lot of traders are anticipating that the market will ghost down from August to September. Does it really go down or is it just a perception? You can find out quick details by looking at the chart below. 

Here show the annual returns of stock if we go Long on Ghost Month


SM

![Full-width image](/assets/img/blog/seasonality/sm-ghost.png){:.lead data-width="800" data-height="100"}

BDO 

![Full-width image](/assets/img/blog/seasonality/bdo-ghost.png){:.lead data-width="800" data-height="100"}

### Turn of Month
Stock returns have tended to be higher in the days before and after the end of the month.


**PAPER**: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=917884
{:.message}

This part is highly intuitive to look at, we should expect a high returns of the first and last trading day of the month. 

![Full-width image](/assets/img/blog/seasonality/smbdo-firstday.png){:.lead data-width="800" data-height="100"}
![Full-width image](/assets/img/blog/seasonality/smbdo-lastday.png){:.lead data-width="800" data-height="100"}


Nice, the chart looks good though there are some drawdowns on BDO for January, March, and August for the first trading day of the month and a huge drawdown for SM on May then minimal on October, not perfect but good in general. For the end of the month, negative returns only in January and December and SM has another huge negative on November and May. Can we say that we are underlying seasonality on every Turn of the Month? can we profit out of these insights? Who knows maybe it is or isn't the only way to find out is to backtest and that's another topic that will be covered in the future.


### Announcement Days
Average asset returns tend to be higher on earnings announcement days. 

Also,/assets tend to trend strongly ahead of important information announcements. So you might want to look at trading short term momentum strategies on:

+ Earnings Announcement
+ Economic Data Annoucement
+ Board Meetings
+ Supply/Demand reports.
 
**PAPER**: https://www.aqr.com/Insights/Research/Journal-Article/Pronounced-Momentum-Patterns-Ahead-of-Major-Events
{:.message}

This strategy focuses on market psychology and historical data. When traders peek into the past data such as quarterly earnings reports they likely to believe that this will affect the prices. By becoming familiar with the specific market traders can make an educated guess as to whether a stock price will increase or discrete following the news report. Now, this is quite common some traders though the main questions still lie on how fast does the price reacts based on these announcements? Right away? Week delay? or won't react. You cannot say that it is very simple to trade on this type of seasonality where you just buy when there's a good report and sell when it is bad. Of course, let's see on historical data if announcement days are consistent.

Here is some of the  historic price curve of BDO on every Quarterly Report

![Full-width image](/assets/img/blog/seasonality/bdoq2.png){:.lead data-width="800" data-height="100"}
![Full-width image](/assets/img/blog/seasonality/bdo2018anual.png){:.lead data-width="800" data-height="100"}

Feel free to check this out on investagrams and share what you have observed. Did the reports reflect on the change of price as expected? How do we anticipate these future result before the announcement? 

Okay so we've run through some of the most popular seasonality and provided some examples on how to view them in a different perspective, I hope it helped you add to your knowledge for making good investment options. As always remember to embrace the uncertainty of the market since it is a sea of noise it is difficult to find an edge on the market if we are just trading blindly without proper economic explanation and backed up with data and evidence its okay to get only a rough insight of the market direction but be always careful of your actions.

Before we part let me provide you other seasonalities that you can investigate yourself. 

### Holidays
Equity returns is higher just before major holidays.


**BOOK**: Ilmanen Expected Returns: Chapter 25 (https://www.amazon.com/Expected-Returns-Investors-Harvesting-Rewards/dp/1119990726)
{:.message}

### Supply and Demand Seasonality
We’d expect spot commodity prices to change based on predictable changes in the supply-demand such as storm incoming and the demand for oil increasing. 

We still seem to be able to make money by:

+ Buying agricultural commodities after the harvest (high supply) and selling before (scarce supply)
+ Buying / selling oil based on demand patterns.


### Monthly Periodic
Individual stocks seem to underperform or overperform in the same month each year. For a while, anyway.


**PAPER**: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=687022
{:.message}

### Intraday Seasonality
Intraday patterns can be tough to exploit due to the costs of trading.

**PAPER**: https://www.snb.ch/n/mmr/reference/working_paper_2011_04/source/working_paper_2011_04.en.pdf
{:.message}

