# Tableau Project: British Airways Reviews

## Project Overview

In this documentation, I explain how I created an interactive Tableau dashboard. The project aims to build a dashboard that lets users explore and visualize data from British Airways reviews, with options for various filters and parameters.

## Objective

My main goal was to showcase my data visualization skills in Tableau through an interactive dashboard that allows:

- **Dynamic metric selection**: Users can choose metrics like overall ratings and cabin staff service.
- **Geographical representation**: Users can view reviews on a map.
- **Comprehensive filtering**: Users can filter reviews by date, travel type, seat type, and aircraft.

## Project Components

- **Data Sources**:
  - **BA Reviews**: This contains reviews with details like author, date, place, ratings, etc.
  - **Countries**: This maps countries to continents and regions.

- **Tools Used**:
  - **Tableau**: I used this for creating the dashboard.
  - **Text Editor**: I used this for documenting steps and notes.

## Data Preparation

### Data Connection

I loaded the CSV files into Tableau:
- **BA Reviews**: I imported the reviews dataset.
- **Countries**: I imported the country mapping dataset.

### Data Relationships

I connected the BA Reviews and Countries datasets using the **place** column from the reviews to the **country** column in the Countries table. This enables geographical filtering.

## Dashboard Development

### Dashboard Layout

- The dashboard features an interactive design with metrics and filters.
- Visual elements include a map, summary metrics, and filter panels.

### Adding Interactivity

1. **Creating Metrics Parameter**:
   - I set up a parameter called "Pick a Metric" for users to choose different metrics.

2. **Creating a Calculated Field**:
   - I used a **CASE** statement to create a field called "Metric Selected" based on the user’s choice.

3. **Dynamic Title**:
   - I made a title that updates according to the selected metric (e.g., “Average [Selected Metric] by Country”).

### Filter Implementation

1. **Creating Date Filter**:
   - I added a date filter in continuous month format for time selection.

2. **Other Filters**:
   - I created filters for:
     - **Seat Type**: Business, economy, or all.
     - **Traveler Type**: Different traveler categories.
     - **Aircraft**: Most reviewed aircraft, grouping less common types as “Various.”

## Finalization

### Dashboard Refinement

- I organized filters logically.
- I ensured all filters work correctly and enhanced usability with thoughtful design choices.

### Testing

- I tested all filters and parameters to confirm they function as expected and all visual elements update properly.

## Conclusion

This Tableau project demonstrates my ability to create effective data visualizations through an interactive dashboard, enhancing user experience with dynamic metrics and filtering options. This documentation serves as a guide for recreating the project and can be useful for my future data visualization efforts.

