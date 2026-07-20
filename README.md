# WalkCalendar - Walking Route Calendar

A clean, interactive single-page application for planning and visualizing your walking routes on a calendar. Perfect for fitness enthusiasts, urban explorers, or anyone who wants to track their daily walks with location-based route details.

<img width="1880" height="1916" alt="image" src="https://github.com/user-attachments/assets/d0d1319c-086d-4948-b35b-887f036acc4b" />

## Features

- ** Interactive Calendar View** - Browse months and see all your planned walking routes at a glance
- ** Route Details Panel** - View comprehensive information about each route including title, distance, duration, and description
- ** Location Preview** - Visual map placeholder that dynamically updates with route information
- ** Add New Routes** - Easily create new walking routes for any date with a simple form prompt
- ** Today's View** - Jump directly to today's date with one click
- ** Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- ** Clean UI** - Modern, intuitive interface with visual indicators for route availability

## Technology Stack

- **HTML5** - Semantic markup structure
- **CSS3** - Custom styling with Flexbox and CSS Grid
- **Vanilla JavaScript** - No frameworks, pure DOM manipulation
- **Font Awesome 6** - Icon library for visual enhancements
- **Google Fonts (Inter)** - Clean, modern typography

## Usage

### Navigating the Calendar
- Use the **Prev/Next** buttons to switch months
- Click **Today** to return to the current date
- The current month and year are displayed at the top

### Viewing Routes
- **Highlighted days** (blue background) indicate routes exist
- Click any highlighted day to view its route details
- The route panel updates with:
  - Route title
  - Distance
  - Duration
  - Description
  - Location preview

### Adding a New Route
1. Click a day on the calendar (it doesn't need to have a route)
2. Click the **Add Route** button
3. Fill in the prompt fields:
   - Route title
   - Distance (e.g., "4.2 km")
   - Duration (e.g., "48 min")
   - Description (optional)
4. The route will be saved and the calendar will update instantly

### Sample Data
The application comes pre-populated with sample routes for March 2026 to demonstrate functionality. You can add, modify, or delete these as needed.

## Project Structure

```
walkcalendar/
├── index.html          # Main application file (includes all CSS and JS)
├── README.md           # Project documentation
└── assets/             # (Optional) Images and other assets
```

## Customization

### Modifying Sample Routes
The sample routes are stored in the `seedSampleRoutes()` function in the JavaScript section. To customize:

```javascript
const samples = [
  { 
    date: '2026-03-04', 
    title: 'Your route title', 
    distance: '5.0 km', 
    duration: '45 min', 
    description: 'Your route description' 
  },
  // Add more routes...
];
```

### Changing the Location Badge
Update the location display in the HTML:
```html
<span id="currentLocationDisplay">Your City, State</span>
```

### Styling Modifications
All styles are contained within the `<style>` tag. Key variables to customize:
- Primary color: `#2a7de1` (buttons, highlights)
- Background colors: `#f5f7fb`, `#ffffff`
- Font family: 'Inter' (can be changed in Google Fonts link)

## Responsive Breakpoints

- **Desktop**: Full layout with side-by-side panels
- **Tablet (700px)**: Stacked panels, smaller calendar cells
- **Mobile (480px)**: Compact header, reduced font sizes, touch-friendly targets

## Roadmap

- [ ] Persistent storage with localStorage
- [ ] Export/Import routes as JSON
- [ ] Actual map integration (Google Maps/Leaflet)
- [ ] Route editing and deletion
- [ ] Route categories/tags
- [ ] Statistics dashboard (total distance, walks per month)
- [ ] Share routes with others
- [ ] Weather integration for route planning

## Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

Please ensure your code follows the existing style and includes appropriate comments.

## Bug Reports

If you find a bug, please open an issue with:
- A clear description of the problem
- Steps to reproduce
- Expected vs. actual behavior
- Screenshots if applicable
- Browser and version information

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Font Awesome](https://fontawesome.com/) for the beautiful icons
- [Google Fonts](https://fonts.google.com/) for the Inter typeface
