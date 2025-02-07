# Responsive Grid Layout

This project demonstrates the implementation of a responsive grid layout using CSS Grid. The layout adjusts dynamically across different screen sizes, showcasing a simple grid structure with 4 columns, which adapts to mobile, tablet, and desktop viewports.

## Project Structure

- **index.html**: The main HTML file containing the structure of the grid and columns.
- **css/**
  - **main.css**: The primary CSS file for styling the grid layout, including responsive grid settings and media queries.
  - **grid.css**: Contains additional grid-specific styles, including media queries for different screen sizes.

## Features

- A responsive grid layout with the following configurations:
  - **Mobile (max-width: 640px)**: The layout is a single column.
  - **Tablet (min-width: 641px)**: The layout uses a 4-column grid.
  - **Desktop (min-width: 1200px)**: The grid switches to a 12-column layout.

- **Column Visibility**: Based on the screen size:
  - **Mobile**: Columns 3 and 4 are hidden.
  - **Tablet and Desktop**: All columns (1-4) are visible.

- **Background Colors**: Each column has a unique background color that changes based on the screen size:
  - **Mobile**: Columns 1 and 2 have background colors (blue and purple).
  - **Tablet**: Columns 3 and 4 also display with background colors (grey and brown).

## How It Works

1. **HTML Structure**: The grid is defined in the `index.html` file using `div` elements, each with specific column classes like `col-1`, `col-2`, `col-3`, and `col-4`.
2. **CSS Grid Layout**: The `grid-con` class defines the grid, while column spans and media queries are used to control the layout for different screen sizes.
3. **Responsive Design**:
   - On mobile (max-width 640px), the grid displays in a single column.
   - On tablets (min-width 641px), the grid adapts to a 4-column layout.
   - On desktops (min-width 1200px), the layout adjusts to a 12-column grid.

## Media Queries

- **Mobile (max-width: 640px)**: 
  - Displays a single column layout (`grid-template-columns: 1fr`).
  - Hides columns 3 and 4 using `display: none`.
  
- **Tablet (min-width: 641px)**: 
  - Displays a 4-column layout (`grid-template-columns: repeat(4, 1fr)`).
  - Displays columns 1, 2, 3, and 4 with specified background colors.
  
- **Desktop (min-width: 1200px)**: 
  - The grid uses 12 equal columns (`grid-template-columns: repeat(12, 1fr)`).
  - Columns 1, 2, 3, and 4 remain visible, with specific background colors.

## Instructions

To view the project:

1. Clone or download the repository.
2. Open the `index.html` file in your browser to see the responsive grid layout in action.

## License

This project is open source and available under the [MIT License](LICENSE).
