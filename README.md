# Tableau Project: British Airways Reviews

## Project Overview

This documentation explains how to create an interactive Tableau dashboard. The project aims to build a dashboard that lets users explore and visualize data from British Airways reviews, with options for various filters and parameters.

## Objective

The main goal is to showcase data visualization skills in Tableau through an interactive dashboard that allows:

- **Dynamic metric selection**: Choose metrics like overall ratings and cabin staff service.
- **Geographical representation**: View reviews on a map.
- **Comprehensive filtering**: Filter reviews by date, travel type, seat type, and aircraft.

## Project Components

- **Data Sources**:
  - **BA Reviews**: Contains reviews with details like author, date, place, ratings, etc.
  - **Countries**: Maps countries to continents and regions.

- **Tools Used**:
  - **Tableau**: For creating the dashboard.
  - **Text Editor**: For documenting steps and notes.

## Data Preparation

### Data Connection

Load the CSV files into Tableau:
- **BA Reviews**: Import the reviews dataset.
- **Countries**: Import the country mapping dataset.

### Data Relationships

Connect the BA Reviews and Countries datasets using the **place** column from the reviews to the **country** column in the Countries table. This enables geographical filtering.

## Dashboard Development

### Dashboard Layout

- The dashboard features an interactive design with metrics and filters.
- Visual elements include a map, summary metrics, and filter panels.

### Adding Interactivity

1. **Creating Metrics Parameter**:
   - Set up a parameter called "Pick a Metric" for users to choose different metrics.

2. **Creating a Calculated Field**:
   - Use a **CASE** statement to create a field called "Metric Selected" based on the user’s choice.

3. **Dynamic Title**:
   - Make a title that updates according to the selected metric (e.g., “Average [Selected Metric] by Country”).

### Filter Implementation

1. **Creating Date Filter**:
   - Add a date filter in continuous month format for time selection.

2. **Other Filters**:
   - Create filters for:
     - **Seat Type**: Business, economy, or all.
     - **Traveler Type**: Different traveler categories.
     - **Aircraft**: Most reviewed aircraft, grouping less common types as “Various.”

## Finalization

### Dashboard Refinement

- Organize filters logically.
- Ensure all filters work correctly and enhance usability with thoughtful design choices.

### Testing

- Test all filters and parameters to confirm they function as expected and all visual elements update properly.

## Conclusion

This Tableau project demonstrates effective data visualization through an interactive dashboard, enhancing user experience with dynamic metrics and filtering options. This documentation serves as a guide for recreating the project and can be useful for future data visualization efforts.
