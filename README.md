# Plotly-Express-Data-Visualization
An end-to-end data visualization project using **Plotly Express** and the **Gapminder dataset**, showcasing how to build interactive, animated, and insightful visualizations with minimal code.

## Project Overview
This project demonstrates the power of modern data visualization using **Plotly Express**, a high-level interface for creating interactive visualizations in Python. Inspired by Hans Rosling’s iconic Gapminder presentation, this notebook explores global development trends such as:
- Life Expectancy
- GDP per Capita
- Population Growth
- Geographic Patterns

The project walks through progressively advanced visualizations, from simple bar charts to animated global maps.

## Dataset
**Source:** Gapminder dataset (built into Plotly Express)

**Accessed via:** `px.data.gapminder()`

**Features include:**
- Country
- Year
- Population (`pop`)
- GDP per capita (`gdpPercap`)
- Life expectancy (`lifeExp`)
- Continent
- ISO country codes (`iso_alpha`)

## Project Structure & Tasks
### Task 1: Loading the Data
- Imported required libraries (`pandas`, `plotly`, etc.)
- Loaded Gapminder dataset using Plotly Express
- Displayed dataset preview using `create_table`

### Task 2: Quick Visualizations with Custom Bar Charts
- Created bar charts for **Canada’s population over time**
- Enhanced visualization with:
  - Color encoding (`lifeExp`)
  - Hover data (`gdpPercap`, `lifeExp`)
  - Custom labels

### Task 3: Life Expectancy vs GDP per Capita
- Built scatter plots to explore relationship between GDP and life expectancy
- Added:
  - Color grouping by continent
  - Automatic legend handling

### Task 4: Interactive Bubble Charts
- Extended scatter plots into **bubble charts**
- Features:
  - Bubble size scaled by population
  - `hover_name` to identify countries
- Enables intuitive exploration of outliers and trends

### Task 5: Animations & Facet Plots
- Created **facet plots** by continent
- Applied logarithmic scaling (`log_x=True`)
- Built animated scatter plots:
  - `animation_frame="year"`
  - `animation_group="country"`
- Added:
  - Axis ranges for smooth animation
  - Clean labels across the visualization

### Task 6: Geographic Visualizations (Maps)
- Built animated **choropleth maps**
- Features:
  - Life expectancy represented by color
  - Time-based animation
  - Multiple projections:
    - Natural Earth
    - Orthographic (globe view)

### Task 7: Line & Area Plots
- Created:
  - **Line plots** for life expectancy trends
  - **Area plots** for population growth
- Used:
  - `line_group` for country-level tracking
  - Smooth curves (`line_shape="spline"`)

## Key Features
- Interactive plots (zoom, hover, select)
- Animated visualizations over time
- Multi-dimensional encoding (color, size, facets)
- Geographic mapping capabilities
- Minimal code with powerful output
