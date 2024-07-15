---
title: 'Population change of 300 US cities between 2020 and 2024'
description: 'The impact of COVID-19 pandemic in figures'
---

*By [César Heredia](https://x.com/cahered), data journalist*



### The kings of Europe
<PlotlyBarChart
  data={{
    url: 'winners.csv'
  }}
  title="Spain surpassed Germany as the most winning country"
  xAxis="winner"
  yAxis="championships"
/>


### Winning rates of countries in European Championships*
<FlatUiTable
  data={{
    url: 'rate_win_country.csv'    
  }}
/>


### Goals scored by match in European Championships
<PlotlyLineChart
  data={{
    url: 'goals_match.csv'
  }}
  title="France vs. Yugoslavia, held in 1960, is the match with the most goals scored*"
  xAxis="match"
  yAxis="goals_scored"
/>
