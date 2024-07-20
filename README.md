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

Ninety-five cities from 29 US states have seen their population diminish between 1K and 9K. Twenty-nine out of these 95 cities belong to California. No other state registered more than seven cities with such losses.

<PlotlyBarChart
  data={{
    url: '1k_loss.csv'
  }}
  title="US cities that lost +1K population in 2024 compared to 2020"
  xAxis="city_state"
  yAxis="pop_loss"
/>

The population of 38 out of the 300 selected cities changed between -1,000 and 1,000 since 2020. Among them are Pittsburgh (PA), Dallas and border-city El Paso (TX), Jersey City (NJ), and five Californian cities.

<PlotlyBarChart
  data={{
    url: 'change_btw_-1k_1k.csv'
  }}
  title="US cities that population has changed between -1K and 1K"
  xAxis="city_state"
  yAxis="pop_loss"
/>

<PlotlyBarChart
  data={{
    url: '1k_won.csv'
  }}
  title="US cities that population has increased between 1K and 10K"
  xAxis="city_state"
  yAxis="pop_won"
/>

## Full data

<FlatUiTable
  data={{
    url: 'data.csv'    
  }}
/>

<PlotlyBarChart
  data={{
    url: 'pop_above_500k.csv'
  }}
  title="US cities with population above 500K people in 2024"
  xAxis="city"
  yAxis="population_2024"
/>

<PlotlyBarChart
  data={{
    url: 'popup_below_500k.csv'
  }}
  title="US cities with population below 500K people in 2024"
  xAxis="city"
  yAxis="population_2024"
/>




<PlotlyBarChart
  data={{
    url: '10k_pop_won.csv'
  }}
  title="US cities that registered +10K population in 2024 compared to 2020"
  xAxis="city"
  yAxis="population_won"
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

<Vega
  data={{
    table: [
      {
        x: "NY-2020",
        y: 8740292
      },
      {
        x: "NY-2024",
        y: 8097282
      },
      {
        x: "LA-2020",
        y: 3895848
      },
      {
        x: "LA-2024",
        y: 3795936
      },
      {
        x: "CHI-2020",
        y: 2743329
      },
      {
        x: "CHI-2024",
        y: 2638159
      },
      {
        x: "HOU-2020",
        y: 2299269
      },
      {
        x: "HOU-2024",
        y: 2319119
      },
      {
        x: "PHX-2020",
        y: 1612459
      },
      {
        x: "PHX-2024",
        y: 1662607
      },
      {
        x: "PHI-2020",
        y: 1600684
      },
      {
        x: "PHI-2024",
        y: 1533828
      },
      {
        x: "SA-2020",
        y: 1439257
      },
      {
        x: "SA-2024",
        y: 1513974
      },
      {
        x: "SD-2020",
        y: 1386292
      },
      {
        x: "SD-2024",
        y: 1388996
      },
      {
        x: "DAL-2020",
        y: 1303212
      },
      {
        x: "DAL-2024",
        y: 1302753
      },
      {
        x: "JAX-2020",
        y: 951880
      },
      {
        x: "JAX-2024",
        y: 997164
      }
    ]
  }}
  spec={{
    $schema: 'https://vega.github.io/schema/vega-lite/v4.json',
    title: "Population change in US major cities",
    data: {
      name: 'table'
    },
    encoding: {
      x: {
        field: 'x',
        title: 'Cities',
        type: 'ordinal'
      },
      y: {
        field: 'y',
        title: 'Population',
        type: 'quantitative'
      }
    },
    mark: 'bar'
  }}
/>
