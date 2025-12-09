# Chasing the Emerald - Seattle Air Travel Visualization

Interactive scrollytelling visualization exploring air travel patterns to Seattle-Tacoma International Airport.

**Created by:** [Suk Jin Chung](https://www.linkedin.com/in/suk-jin003/), [Yongxi Chen](https://www.linkedin.com/in/yongxi-chen-0267b42b7/), [Cecelia Deng](https://www.linkedin.com/in/qdengcecelia/)

## Overview

This project explores flight patterns to Seattle through an interactive scrolling narrative. Users discover transportation evolution, popular routes, major airlines, growth trends, optimal booking times, and flight reliability patterns.

## Project Structure

```
├── index.html              # Main HTML file
├── css/
│   ├── bootstrap.min.css
│   └── style.css          # Custom styles
├── js/
│   ├── helpers/           # Core functionality
│   │   ├── data_loader.js
│   │   ├── scroller.js
│   │   ├── sections.js
│   │   └── visual_controller.js
│   └── sketches/
│       ├── sketch_manager.js
│       ├── sketch_renderer.js
│       └── viz/           # Visualization modules
│           ├── viz_travel.js         # Transportation evolution
│           ├── viz_origins.js        # Route map
│           ├── viz_airline.js        # Airline comparison
│           ├── viz_c.js              # Growth trends
│           ├── viz_pricing.js        # Price calendar
│           └── viz_delay_calendar.js # Flight reliability
├── assets/
│   └── map.png            # Map background
└── data/
    └── seattle_flight_data.js  # Unified dataset
```

## Visualizations

1. **Transportation Evolution** - Comparison of travel times from NYC to Seattle across 1800s (ship), 1900s (train), and today (plane)
2. **Popular Routes** - Interactive map showing top 10 origins for flights to Seattle
3. **Airline Comparison** - Bar chart of the 5 most popular airlines serving Seattle
4. **Growth Trends** - Line chart showing airline flight volume growth from 2010-2019
5. **Price Calendar** - Color-coded guide showing best months and days to book flights
6. **Flight Reliability Calendar** - Visual representation of delay and cancellation patterns throughout the year

## Technology Stack

- **p5.js** - Visualization library
- **Scrollama** - Scroll-driven interactions
- **Bootstrap** - CSS framework
- Vanilla JavaScript

## Data Sources

### Primary Data
- Bureau of Transportation Statistics (BTS) - Airline On-Time Performance Data (T-100 Segment), 2019-2025
- Bureau of Transportation Statistics (BTS) - Average Domestic Air Fares
- Kaggle (Patrick Zel) - Flight Delay and Cancellation Dataset, 2019-2023
- Kaggle (Umer Adnaan) - Flight Delays Dataset
- RowZero - Flights Dataset
- KAYAK - Flight Routes to Seattle-Tacoma International Airport
- Google Flights, Expedia - Pricing patterns (2022-2025 average)

### Historical Context
- Hatton, T. J., & Williamson, J. G. (2004). Voyage Durations in the Age of Mass Migration. CEPR VoxEU
- HISTORY.com - Transcontinental Express Crosses Nation in 83 Hours (1876)
- U.S. Census Bureau (2023) - The Transcontinental Railroad

## Setup

1. Clone the repository
2. Open `index.html` in a web browser
3. Or use a local server: `python -m http.server 8000`

## Features

- Smooth scroll-based storytelling
- Interactive hover tooltips
- Animated transitions
- Responsive visualizations
- Clean, accessible design
