---
title: 'Population change of 300 US cities between 2020 and 2024'
description: 'The impact of COVID-19 pandemic in figures'
---

*By [César Heredia](https://x.com/cahered), data journalist*

<FlatUiTable
  data={{
    url: 'data.csv'    
  }}
/>

<PlotlyBarChart
  data={{
    url: 'data.csv'
  }}
  title="Most populated cities"
  xAxis="city"
  yAxis="pop_2024"
/>

<PlotlyBarChart
  data={{
    url: '10k_pop_loss.csv'
  }}
  title="US cities that lost +10K population in 2024 compared to 2020"
  xAxis="city"
  yAxis="population_loss"
/>

<PlotlyBarChart
  data={{
    url: '1k_pop_loss.csv'
  }}
  title="US cities that lost +1K population in 2024 compared to 2020"
  xAxis="city"
  yAxis="population_loss"
/>

<PlotlyBarChart
  data={{
    url: 'less_1k_pop_loss.csv'
  }}
  title="US cities that lost less than 1,000 population in 2024 compared to 2020"
  xAxis="city"
  yAxis="population_loss"
/>

<PlotlyBarChart
  data={{
    url: 'less_1k_pop_won.csv'
  }}
  title="US cities that registered more than 1,000 population in 2024 compared to 2020"
  xAxis="city"
  yAxis="population_won"
/>

<PlotlyBarChart
  data={{
    url: '1k_pop_won.csv'
  }}
  title="US cities that registered +1K population in 2024 compared to 2020"
  xAxis="city"
  yAxis="population_won"
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
    url: 'density_4k.csv'
  }}
  title="US cities with density above 4K"
  xAxis="city"
  yAxis="density"
/>

<PlotlyBarChart
  data={{
    url: 'density_2_5k.csv'
  }}
  title="US cities with density between 2.5K and below 4K"
  xAxis="city"
  yAxis="density"
/>

<PlotlyBarChart
  data={{
    url: 'density_less_2_5k.csv'
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
