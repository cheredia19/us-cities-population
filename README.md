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
    url: 'data.csv'
  }}
  title="Density"
  xAxis="city"
  yAxis="pop_density_mile2"
/>

<PlotlyBarChart
  data={{
    url: 'data.csv'
  }}
  title="Change in population between 2020 and 2024"
  xAxis="city"
  yAxis="change_24_20"
/>

<Vega
  data={{
    table: [
      {
        x: "NY2020",
        y: 8740292
      },
      {
        x: "NY2024",
        y: 8097282
      },
      {
        x: "LA2020",
        y: 3895848
      },
      {
        x: "LA2024",
        y: 3795936
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
