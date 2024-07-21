---
title: 'Population change of 300 US cities between 2020 and 2024'
description: 'The impact of COVID-19 pandemic in figures'
---

*By [César Heredia](https://x.com/cahered), data journalist*

New York City has recorded a population loss of **more than 600 thousand people** between 2020 and 2024, according to [data from 300 selected cities in the United States](https://www.kaggle.com/datasets/dataanalyst001/population-of-all-us-cities-2024). Apart from NYC, the population of the other 21 cities from 16 states has declined by more than 10K. Five of those are in California.

<PlotlyBarChart
  data={{
    url: '10k_loss.csv'
  }}
  title="US cities that lost +10K population in 2024 compared to 2020"
  xAxis="city_state"
  yAxis="pop_loss"
/>

However, by rate, San Francisco (CA) was the city that **lost the highest percent of population** in the period above (-0.09%), whiie the highest increase was [New Braunfels (TX)](https://newbraunfels.gov), located in Comal county. Their inhabitants rose by 91,643 to 117,396, a growth of 0.28%.

Ninety-five towns from 29 US states have seen their population diminish between 1K and 9K. Twenty-nine out of these 95 cities belong to California. No other state registered more than seven cities with such losses.

<PlotlyBarChart
  data={{
    url: '1k_loss.csv'
  }}
  title="US cities that lost +1K population in 2024 compared to 2020"
  xAxis="city_state"
  yAxis="pop_loss"
/>

The population of 38 out of the 300 selected cities **changed between -1,000 and 1,000** since 2020. Among them are Pittsburgh (PA), Dallas and border-city El Paso (TX), Jersey City (NJ), and five Californian cities.

<PlotlyBarChart
  data={{
    url: 'change_btw_-1k_1k.csv'
  }}
  title="US cities that population has changed between -1K and 1K"
  xAxis="city_state"
  yAxis="pop_loss"
/>

Other 98 areas across 29 selected US states expanded from 1,000 to 10,000 people in four years. **37.9% of them are in Texas or California**, including Arlington (TX), Sacramento, and San Diego (CA).

<PlotlyBarChart
  data={{
    url: '1k_won.csv'
  }}
  title="US cities that population has increased between 1K and 10K"
  xAxis="city_state"
  yAxis="pop_won"
/>

In the meantime, the population of 47 cities from 16 states climbed by ten or more thousand between 2020 and 2024. 11 Texan cities entered this group. **San Antonio recorded the largest increase** (+74K) of the 300 analyzed in this report.

<PlotlyBarChart
  data={{
    url: '10k_won.csv'
  }}
  title="US cities that registered +10K population in 2024 compared to 2020"
  xAxis="city_state"
  yAxis="pop_won"
/>

## Most and least populated cities

According to data, 38 of the 300 selected cities recorded a population greater than 500,000 people in 2024, with New York City as the most populated of all. Los Angeles and Chicago complete the podium, despite losing around 100K each.

<PlotlyBarChart
  data={{
    url: '500k_more.csv'
  }}
  title="US cities with population above 500K people in 2024"
  xAxis="city_state"
  yAxis="population"
/>

<PlotlyBarChart
  data={{
    url: 'popup_below_500k.csv'
  }}
  title="US cities with population below 500K people in 2024"
  xAxis="city"
  yAxis="population_2024"
/>

## Full data

<FlatUiTable
  data={{
    url: 'data.csv'    
  }}
/>



<PlotlyBarChart
  data={{
    url: 'pop_density_4k.csv'
  }}
  title="US cities with density above 4K"
  xAxis="city"
  yAxis="density"
/>

<PlotlyBarChart
  data={{
    url: 'pop_density_2_5k.csv'
  }}
  title="US cities with density between 2.5K and below 4K"
  xAxis="city"
  yAxis="density"
/>

<PlotlyBarChart
  data={{
    url: 'pop_density_less_2_5k.csv'
  }}
  title="US cities with density below 2.5K"
  xAxis="city"
  yAxis="density"
/>
