---
layout: post
title: Why College Running Backs are Smart to go Pro Early. Survival Analysis Using KM-Estimation.
---

Conventional wisdom has it that running backs have short careers. So much so that it is in the best interest of elite college football RB's such as Dalvin Cook ( and players at other positions) to go pro as early as possible. The purpose of this post is to see if one can show, using publicly available data, that this is the case. To do this I used a statistical technique called survival analysis.

Survival analysis is a technique that is focused on modeling the time until an event. The event of interest can be a number of things: death, occurrence of a disease, divorce, marriage, finding a job, changing a job, failure of a part, etc. These techniques were initially used in the medical field so death was the event of interest. This is where the name survival analysis came from. In this case, I used the time until retirement or release from a team to determine to probability of remaining in the league for a specific number of seasons.

The data for this analysis comes from the Pro Football Reference.com(http://www.pro-football-reference.com) website where I used the data of 1230 running backs from 1970 to 2014. In using this data I am assuming that a running back made the team. This includes players that were starters and non-starters.

To do the analysis I used what is called Kaplan-Meier Estimation. It is a way of calculating the probability of remaining in the league for x number of seasons. You do this by dividing the number of players that are released/waived/cut or retire during a season by the number of players remaining in the league after that season. 

Here is the equation that we use for K-M Estimation:

$$\hat{S}(t) = \prod_{i:t_i \le t} \left(1-\frac{d_i}{n_i}\right)$$

Where: 
* \\(\hat{S}(t)\\)-The probability of remaining in the NFL at the end of season t.
* \\(t_i\\) - Season where at least one retirement/release has happened.
* \\(d_i\\) - The number of retirements/releases occurring at season t.
* \\(n_i\\) - The number of players that are still in the NFL at season t. 

The product symbol, \\(\prod\\), tells you that you have to multiply everything after the symbol.  So basically you are multiplying the fraction of players remaining in the league in year *n+1* by the fraction remaining in year *n*.  This is done repeatedly for every year.

Here is an example: Let's say that we start out with 100 RB's.  After year 1, 75 remain.  After year 2, 60 remain. After year 3, 50 remain.  To find the survival probabilities after every year we do the following calculation:

* Year 1: \\(\hat{S}(t) = 1-\frac {100-75}{100} = 1-\frac{25}{100} = \frac{75}{100} = 0.75\\) 
 
* Year 2: \\(\hat{S}(t) =(0.75) (1-\frac {75-60}{75}) =(0.75) (1-\frac{15}{75}) = (0.75)(\frac{60}{75}) = (0.75)(0.80) = 0.60\\)

* Year 3: \\(\hat{S}(t) =(0.75)(0.60) (1-\frac {60-50}{60}) =(0.75)(0.80) (1-\frac{10}{60}) = (0.75)(0.80)(\frac{50}{60}) = (0.75)(0.80)(0.8333) = 0.50\\)

At the end of three years, we have a survival probability of 0.50.  This can be extended for as many years as needed.

So what did I find? Figure 1 shows the survival curve for all running backs. The x-axis describes the total number of seasons in the NFL. The y-axis shows the probability of remaining in the league. In this case, the red line shows the probability that half of the 1230 RB's are still in the league. Where this line intersects the survival curve give you the median career length of a running back. This happens after 3 seasons.

<img src="/images/KM_allRB.png" style = "display: block; margin-left: auto;margin-right:auto;" width="400px" height="400px"/>
**Figure 1: Survival Analysis Curve for all NFL Running Backs 1970-2014.** 

Figure 2 shows what happens when you take starting age into account. What you see is that if you start at age 21, the median career length for a running back is 8 seasons. If you start at age 22, this drops to 6 seasons. If you start at age 23, you have a 50 percent chance of lasing just over 5 seasons.

<img src="/images/KM_age.png" style = "display: block; margin-left: auto;margin-right:auto;" width="400px" height="400px"/>
**Figure 2: Survival Analysis Curve for Running Backs 1970-2014 Depending on Starting Age.** 

There are two things that you can take from this analysis: 

1. The career of your average NFL RB is very short.  Three years.
2. You are better off going pro early if you are a star RB in college since your chances of staying in the league are much better the earlier you start.

So what factors other than age affect the longevity of an NFL RB?  That is the subject of another post.


