---
title:  "Taxes now or taxes later"
date:   2019-07-29 08:12:11 -0700
share: true
categories: personal-finance
---

*Disclaimer: I am not a financial professional and this information is only general in nature. Individuals have different financial circumstances and should consult a professional.*

There are many different retirement plans to choose from and it's sometimes hard to determine which one is best for you to choose to reach your retirement goal. I won't go into the details and rules of all the potential plans in this post. Instead, I'll consider a specific question: should you pay taxes now or later? Specifically, we'll compare the future value of contributing the same amount to a traditional 401(k) vs a Roth 401(k).

A traditional 401(k) contribution is tax-deferred. This means that if you put in $100 now, you don't have to pay taxes on $100 of your income this year. However, when you retire and withdraw that money (take a distribution), you will have to pay income tax in the year of withdrawal. This means that for a $100 contribution, it 1) starts in full, 2) grows tax-free for however many years it sits in your retirement account, and then 3) has your future tax rate reduce the future amount.

![401(k) future value model](/../../assets/images/posts/401k_future_value_model.png){: .align-center style="max-width: 600px;"}

*401(k) future value model*
{: style="text-align: center"}

Let's put the traditional 401(k) growth model in equation form so that we can analyze it.

Let $$x$$ be the initial contribution amount. The Contribution portion is just $$x$$.<br />
Let $$r$$ be the expected annual growth rate and $$y$$ be the number of years to grow. Assuming compounding annual growth by $$r$$ for $$y$$ years, the Growth portion is $$x(r^y-1)$$.<br />
Let $$t_1$$ be the future tax rate. The tax rate is applied on the total of the Contribution and Growth. The total Future taxes paid is thus $$t_1(x+x(r^y-1))$$.

Adding these terms together gets us the Future value for the 401(k) model:

$$x+x(r^y-1)-t_1(x+x(r^y-1))$$

$$=x+xr^y-x-t_1x-t_1xr^y+t_1x$$

$$=xr^y-t_1xr^y$$

$$=xr^y(1-t_1)$$

Just for the sake of illustration, let's plug in some numbers. Let's say we contributed $100 initially and left it to grow with 5% annual returns (a 1.05 annual growth rate) for 30 years, and our future tax rate is 25%, the Future value is:

$$ $100 \times 1.05 ^ {30} \times (1-.25) = $432 \times .75 = $324 $$

From this equation, we can see that, ideally, we would want our future tax rate as low as possible to maximize the actual amount we withdraw. This is why most retirees do not withdraw the entirety of their traditional 401(k) in a single year, as much of that withdrawal would fall under high tax brackets. This is also why there is a minimum distribution limit so that retirees don't just let the money sit untaxed forever.

Let's compare this to the same amount, $$x$$, except grown outside of a traditional 401(k) (or any other tax-advantaged account). This means that for an $100 initial contribution, the current tax would have been taken away, and then the amount would have grown over the years. However, this growth rate would be lower than $$r^y$$ since gains outside a tax-advantaged account can be taxed as long term capital gains or as ordinary income.

![no tax advantage model](/../../assets/images/posts/no_tax_advantage_model.png){: .align-center style="max-width: 600px;"}

*No tax advantage model*
{: style="text-align: center"}

Let's put this in equation form too.

We'll define $$t_0$$ to be the current tax rate and $$r^t$$ to be the growth rate with taxes.<br />
The Contribution is still $$x$$.<br />
The Taxes now is just $$t_0x$$.<br />
The Growth (taxed) is $$x(r_t^y-1)$$. Note that we are applying the growth to the full initial contribution. The alternative would be to apply the growth to the contribution amount after Taxes now are applied. However, this would make it an unfair comparison since a lower amount is allowed to grow. The solution is to bring the taxes out into its own term like we have here and then include another cost, which is the lost potential growth on the amount that went to taxes. This lost growth is $$t_0x(r_t^y-1)$$.

Adding these terms together gets us the Future value for the non-tax-advantaged model:

$$x-t_0x-t_0x(r_t^y-1)+x(r_t^y-1)$$

$$=x-t_0x-t_0xr_t^y+t_0x+xr_t^y-x$$

$$=xr_t^y-t_0xr_t^y$$

$$=xr_t^y(1-t_0)$$

Note, however, that if we had just taken the tax out and let the after-tax portion to grow, the resulting Future value would actually still be the same here.

Here, the tax is first taken out from the initial amount at the current tax rate. Compared to the model for the tax-deferred (traditional) 401(k) contribution, the tax-deferred 401(k) contribution is worth it if:

- Your future tax rate $$t_1$$ is lower than your current tax rate, or
- Your future tax rate $$t_1$$ is higher than your current tax rate, but only up to however much is lost from having a lower growth rate ($$r^y/r_t^y>(1-t_0)/(1-t_1)$$)

In the event that your future tax rate is the same as your current tax rate, the traditional 401(k) contribution becomes more worth it as time goes by (since the difference between $$r^y$$ and $$r_t^y$$ increases exponentially as $$y$$ increases) - so contribute early. Also, the tax that you save at present by contributing to your traditional 401(k) is your marginal tax rate, and the tax you pay at withdrawal time would likely be your effective tax rate (that is, if your traditional 401(k) distributions are your main source of retirement income). This means that, most likely, your current tax rate would be higher than your future tax rate for the traditional 401(k) contribution. Unless your future tax rate is significantly higher than your current tax rate or the taxes on growth is just too miniscule, it seems **always better to put the money in the traditional 401(k) than just leaving it without tax advantages**.

Now, let's take a look at the Roth 401(k). Roth 401(k)s have tax-free growth, which means that once you put money into a Roth 401(k), that money can grow tax-free, and you'll never have to pay tax on that money again. When you withdraw that money in retirement, you'll also pay no taxes.

![no tax advantage model](/../../assets/images/posts/roth_401k_model.png){: .align-center style="max-width: 600px;"}

*Roth 401(k) model*
{: style="text-align: center"}

Individuals contribute to a Roth 401(k) with after-tax money. For these contributions, the future value of the Roth 401(k) is the same as the non-tax-advantaged case except that it can enjoy the higher non-taxed growth rate, making it strictly better than leaving money outside. (As a side note, Roth IRAs act the same as Roth 401(k)s, except that normally, only individuals under a certain income threshold can directly contribute to them. This is why direct Roth IRA contributions have a very low limit and individuals with incomes over a certain threshold are not allowed to contribute directly. However, there are a few ways for individuals above the income threshold to contribute a significant amount, including backdoor and mega-backdoor contributions. These methods essentially take after-tax money from different sources and place them into a Roth IRA, and are equivalent to doing a direct contribution. Alright, back to Roth 401(k)s.)

Let's put the Roth 401(k) model in equation form.

The Contribution is $$x$$.<br />
The Taxes now is $$t_0x$$.
The Growth (tax-free) is $$x(r_y-1)$$. Here, we have to subtract the lost growth on the portion paid as taxes as well, which is $$t_0x(r_t^y-1)$$. Note that we use the growth with taxes here since the portion paid to taxes would have grown without tax advantages.

The Future value for the Roth 401(k) model is thus:

$$x-t_0x-t_0x(r_t^y-1)+x(r^y-1)$$

$$=xr^y-t_0xr_t^y$$

This is quite similar to the non-tax-advantaged case except that we have the positive term as $$xr^y$$ instead of $$xr_t^y$$. Even though this seems like a small difference, the difference can be huge as the number of years $$y$$ gets large. For instance, a $100 contribution with 1.05 tax-free growth rate would grow to $704 in 40 years, but only $480 with a 1.04 taxed growth rate. In other words, the 20% annual tax on long-term gains turns into a 32% overall tax after 40 years. (As a side note, if you're following modern portfolio theory, don't rebalance too often even with long-term gains. Having a 1.04 growth rate compared to a 1.05 growth rate every year is a lot less than just paying 20% tax one time.)

Now, let's compare the Roth 401(k) to a traditional 401(k). Let's take a look at the traditional 401(k) model (with the tax cost split out into its own term) alongside the Roth 401(k) model:

$$xr^y-t_1xr^y$$ traditional 401(k) vs. $$xr^y-t_0xr_t^y$$ Roth 401(k)

Now we can compare the traditional 401(k) to Roth 401(k) easily. As you can see, both share a common term $$xr^y$$, the initial amount with growth. The only difference is in the tax cost term. For Roth 401(k), the tax cost is $$t_0xr_t^y$$, whereas for traditional 401(k), the tax cost is $$t_1xr^y. These have a common term $$x$$ that can also be disregarded. We have simplified the comparison between traditional 401(k) and Roth 401(k) to just:

Traditional 401(k) vs Roth 401(k)

$$t_1r^y$$ vs $$t_0r_t^y$$

This looks familiar doesn't it. This is just like comparing the traditional 401(k) model to the no tax advantage model, except here the Roth 401(k) is like the traditional 401(k) and the traditional 401(k) is like the no tax advantage. Comparing the models, the Roth 401(k) contribution is worth it if:

- Your future tax rate $$t_1$$ is higher than your current tax rate, or
- Your future tax rate $$t_1$$ is lower than your current tax rate, but only up to however much is lost from having a lower growth rate ($$r^y/r_t^y>t_0/t_1$$)

Therefore, for young people with many years to compound growth, the Roth 401(k) can be a better option than the traditional 401(k). Just using our $$r^y=1.05$$ and $$r_t^y=1.04$$ from above over a 40 year period, the ratio becomes about $$r^y/r_t^y=1.47$$. It would generally not be the case that $$t_0/t_1>1.47$$. Using some more aggressive growth rates like $$r^y=1.1$$ and $$r_t^y=1.08$$, we get an even larger ratio like 2.08. It would be quite unlikely to have the current marginal tax rate be more than double the future effective tax rate. However, as one gets older, there will be less time for a contribution to grow, and one would favor the traditional 401(k) more and more over the Roth 401(k). **The recommendation is to favor contributions to the Roth 401(k) more when you are young (like before 30) and then exponentially decay that contribution to favor more towards traditional 401(k) as you get older (like after 30).**

<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
