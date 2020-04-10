---
layout: default
title: 2019 nCoV
parent: Research
nav_order: 2
---

# 2019 nCoV

I enjoy exploring and visualizing public datasets, so naturally the novel coronavirus 2019 nCoV caught my attention -- after the initial outbreak in China, the rest of the world is now struggling with massive contagion and the situation has now been classified as a pandemic:

![](/assets/images/cases_total.png){:width="900px"}
![](/assets/images/deaths_total.png){:width="900px"}

Clearly, the spread of the disease has really accelerated outside of China since late February. This can be seen in more detail on a per-country basis:

![](/assets/images/cases_top10.png){:width="900px"}

The slope of the growth in cases is currently steepest in the US, while it is flat in China. This can also be seen in the daily increase in cases (lower panel). In terms of deaths, however, Italy and Spain currently face the most dire situation:

![](/assets/images/deaths_top10.png){:width="900px"}

However, if we account for differences in population, the situation looks a bit different:

![](/assets/images/cases_top10_pc_min0.png){:width="900px"}
![](/assets/images/deaths_top10_pc_min0.png){:width="900px"}

San Marino and the Holy See (aka Vatican City) are geographically within Italy, and Andorra lies between Spain and France, so this is not too surprising given their locations and small populations. Iceland also has a small population, but is in the process of testing all citizens, so their numbers are likely to be more complete (accurate). Dominica, however, is located in the Caribbean and has a small population, but their numbers may not be reliable.
If we now consider only countries with a population above 100,000 people, we get the following:

![](/assets/images/cases_top10_pc_min100000.png){:width="900px"}
![](/assets/images/deaths_top10_pc_min100000.png){:width="900px"}

We can learn more about the differences in severity between different countries by plotting growth curves. As we saw above, the US is currently leading the world in terms of the total number of cases, but also in terms of how fast the number of cases is growing. However, to really see how the growth trend in the US compares to other countries, we need to plot the curves starting from a common reference time that is independent of the (somewhat random) time the disease was imported in significant numbers. In the following plot, we choose this time (somewhat arbitrarily) to be the day that the number of cases reached 100:

![](/assets/images/cases_rate_top10.png){:width="900px"}

China is a notable outlier in this plot, having faced a larger growth rate earlier in the outbreak than other countries, but this is likely due to the fact that the outbreak started there, so it had longer time to spread before the authorities began implementing containment measures. However, we can make the same kind of plot for the number of deaths instead of cases, and now we see that China is no longer an outlier:

![](/assets/images/deaths_rate_top10.png){:width="900px"}

This is perhaps surprising given the extremely fast growth in cases early on in China, but could potentially be explained by the rapid construction of new hospitals in Wuhan, or by misdiagnoses, reporting "noise", or a combination of factors.
