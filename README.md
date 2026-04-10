# Global GDP per Capita — Animated Choropleth Map

Animated world map showing GDP per capita from 1952–2007, built entirely in R.

![GDP Map Animation](gdp_map.gif)

## Features

- **[Equal Earth projection](https://equal-earth.com/equal-earth-projection.html)** — accurate area representation
- **[Box-Cox transformation](https://quantitudepod.org/s4e17-box-cox/)** — optimal scaling for skewed GDP data
- **Animated timeline** — smooth transitions across years with progress bar
- **Globe outline** — ocean background with [graticule](https://en.wikipedia.org/wiki/Graticule_(cartography)) grid
- **Country boundaries** — visible border lines between nations with official India boundary via [Natural Earth](https://www.naturalearthdata.com/downloads/)

## Requirements

```r
install.packages(c("here", "ggplot2", "gganimate", "sf", "maps",
                    "dplyr", "gifski", "gapminder", "scales", "MASS"))


## Usage

```r
source("gdp_map.R")
```

The script outputs `gdp_map_v9.gif` in your working directory.

## Data Source

- [Gapminder](https://www.gapminder.org/) — GDP per capita (1952–2007)

## Static Preview

![Static Map](static.jpeg)
