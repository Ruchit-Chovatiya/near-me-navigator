# near-me-navigator
Category-based nearby facility finder using Geoapify and OpenStreetMap.
# NearMe Navigator — near.me

A category-based nearby facility finder that helps users discover cafés, pharmacies, ATMs, and bus stops around a selected location.

**Live Website:** https://ruchit-chovatiya.github.io/near-me-navigator/

## About the Project

NearMe Navigator is a web application developed as part of a Full Stack Development project. It provides a simple way to search for nearby facilities without navigating through a complex map interface.

Users can enter a destination, select a category, and view nearby places in an organized card layout. Each result includes available location details and a direct link to OpenStreetMap.

## Features

- Search for a location by name or address.
- Discover nearby cafés, pharmacies, ATMs, and bus stops.
- Search within a 3 km radius.
- Display up to 75 results per search.
- View place names and available address information.
- Open individual locations directly on OpenStreetMap.
- Responsive interface for desktop and mobile screens.
- Loading messages and error handling for API requests.

## Technologies Used

- **HTML5** — Page structure
- **CSS** — Styling and layout
- **Tailwind CSS** — Responsive interface design
- **JavaScript** — Search logic and API integration
- **Geoapify Geocoding API** — Converts place names into geographic coordinates
- **Geoapify Places API** — Retrieves nearby facilities
- **OpenStreetMap** — Map links and geographic information

## How It Works

1. Enter a destination, such as Christ University, Bengaluru.
2. Select a category from the dropdown menu or category cards.
3. The Geocoding API identifies the destination's coordinates.
4. The Places API searches for matching facilities within 3 km.
5. The application displays up to 75 results.
6. Click **Explore this place** to view a location on OpenStreetMap.

## Getting Started

### Prerequisites

- A modern web browser
- An internet connection
- A Geoapify API key

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Ruchit-Chovatiya/near-me-navigator.git
   ```

2. Open the project folder:

   ```bash
   cd near-me-navigator
   ```

3. Open `index.html` in your browser or run it using the VS Code Live Server extension.

4. Configure your Geoapify API key in the JavaScript configuration before searching.

   ```javascript
   const GEOAPIFY_API_KEY = "YOUR_GEOAPIFY_API_KEY";
   ```

   Replace the placeholder with your own API key.

## API Configuration and Security

NearMe Navigator uses Geoapify services to retrieve geographic information. API requests require a valid key.

Since browser-side JavaScript is visible to visitors, configure appropriate API-key restrictions and monitor usage. For stronger protection, use a backend service to handle API requests instead of exposing an unrestricted key.

## Limitations

- Search results depend on the availability and completeness of geographic data.
- An internet connection is required.
- API availability, usage limits, and key restrictions may affect searches.
- Some locations may have incomplete names or address details.
- The application provides direct map links rather than built-in turn-by-turn navigation.

## Future Enhancements

- Add more facility categories.
- Display results on an interactive map.
- Sort results by distance.
- Allow users to customize the search radius.
- Improve accessibility and mobile usability.
- Add additional error recovery and API service handling.

## Data Attribution

Geographic data and map links are provided through OpenStreetMap.

https://www.openstreetmap.org/

Geoapify API documentation: https://apidocs.geoapify.com/

## Author

**Ruchit Chovatiya**

GitHub: https://github.com/Ruchit-Chovatiya

---

*NearMe Navigator — A little closer to everywhere.*
