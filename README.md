# World Population: Reimagining Data Visualizations in R

An interactive Quarto website that takes a static world population chart and rebuilds it into clearer, explorable visualizations in R.

**Live site:** https://erityperwizz.github.io/world-population-viz/

**Authors:** Erica Mathias and Jeevani Bhaskar

## What's inside

| Page | What it shows |
|---|---|
| **Redesign** | The original static chart rebuilt as two cleaner ggplot2 views that make country and continent comparisons easy to read |
| **Map** | An interactive Leaflet choropleth of population by country. Hover over any country to see its name, population and share of the world |
| **Drill-down** | A Highcharts bar chart of total population by continent. Click a continent to drill down into its countries, sorted largest to smallest |
| **Code** | All R code used to build the visuals, for full reproducibility |

## Data

`countries_population_continents.csv`: population estimates for 240+ countries and territories (2023 to 2024), with each country's share of the world and its continent.

To get every map region shaded, country names in the data were standardized to match the world map's naming (for example *United States* to *USA*, *Eswatini* to *Swaziland*), and multi-island nations such as *Trinidad and Tobago* were mapped to each of their islands.

## Tools

R, Quarto, Leaflet, Highcharter, ggplot2, dplyr, purrr, sf, RColorBrewer

## Run it locally

```r
install.packages(c("leaflet", "highcharter", "ggplot2", "dplyr", "purrr", "readr", "sf", "RColorBrewer", "htmltools"))
```

Then from the project folder run `quarto render`. The site is built into `docs/`, which GitHub Pages serves.
