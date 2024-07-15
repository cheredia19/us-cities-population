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

<PlotlyLineChart
  data={{
    url: 'data.csv'
  }}
  title="Population in 2020 vs 2024"
  xAxis="city"
  yAxis="pop_2020"
/>
