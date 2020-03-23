---
layout: default
title: 2019 nCoV
parent: Research
nav_order: 2
---

# 2019 nCoV

I also enjoy exploring and visualizing public datasets. For example, the novel coronavirus 2019 nCoV caught my attention -- after the initial outbreak in China, the rest of the world is now struggling with massive contagion and the situation has now been classified as a pandemic:

![](/assets/images/ncov0.png){:width="900px"}

While the spread of the disease has apparently stabilized in China, the rest of the world has seen marked increases in transmission rates. This can be seen by looking at the daily increases in confirmed cases over time:

![](/assets/images/ncov1.png){:width="900px"}

Some of the spikes in these curves correspond to changes in diagnosis criteria and reporting policies. In addition to methodology, transparency also varies by country, so the data are fundamentally ``noisy''. Differences in culture and government response may manifest as different contagion trajectories. Ranked by their total number of cases, the top trajectories look like this:

![](/assets/images/ncov2.png){:width="900px"}

However, the linear scale obscures much of the information in the plot, as it is dominated by the large number of cases in China before the disease became a pandemic. By using a logarithmic scale, we can more easily see what's going on:

![](/assets/images/ncov3.png){:width="900px"}

Another way to visualize the spread of the disease is by focusing on the daily increase in cases. Instead of ranking by total number of cases, here we rank by the median daily increase in cases:

![](/assets/images/ncov4.png){:width="900px"}

From this plot it appears that a fundamental shift in the spread of the disease occurred around February 23rd. Before this date, the daily increases are dominated by China, whereas after this date the rest of the world begins to dominate. To better see the spread outside of China, we can now rank by the median daily increase in cases after this date:

![](/assets/images/ncov5.png){:width="900px"}

Early on in this time period, rapid spreading of the disease is seen primarily in South Korea, Iran, and Italy. Later in this time period, rapid growth in confirmed cases is more prominent in Spain, Germany, and the US.
