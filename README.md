# Turn Tables into Animations Using R

Presenting data with temporal and geographic features are often more engaging through animations and maps. This post will give a walkthrough on using R to extract the data from public sources, wrangle the data, and create an animation of a map.

The data we will be using is the [daily weather summaries of 2020](https://digital.nmla.metoffice.gov.uk/SO_72b4d5a3-e5f0-41dc-a31d-1a3c8c4f1f59/) provided by the [Met Office](https://www.metoffice.gov.uk/) (based in the UK). The data is stored as tables within a PDF, which we will have to parse using the `pdftools` package. The exact location (longitude and latitude) of each [weather station](https://www.metoffice.gov.uk/research/climate/maps-and-data/uk-synoptic-and-climate-stations) will be referenced using web-scraping methods from the `rvest` package. To source the country boundary data and coordinates, we will use the `rnaturalearth` package, which sources the coordinates from [Natural Earth](https://www.naturalearthdata.com/).

To manipulate and wrangle the data, we will use the `dplyr` and `tidyverse` toolkit. For the plots, we will use the `ggplot2`, `gganimate`, and `sf` package.

This post will cover:

- PDF parsing
- Web scraping
- Data wrangling
- Plotting maps with `sf`
- Animating plots with `gganimate`

Continue reading at [https://kevinchtsang.github.io/weather-animation/](https://kevinchtsang.github.io/weather-animation/)