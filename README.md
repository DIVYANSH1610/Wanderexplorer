WanderExplorer - Discover Your Dream Destination
WanderExplorer is a dynamic and visually stunning web application designed to help users explore their dream travel destinations. By integrating real-time weather data, high-quality images, and informative summaries, it provides an immersive experience for discovering cities worldwide. Built with HTML, CSS, and JavaScript, WanderExplorer features a responsive design, smooth animations, and a user-friendly interface, making it perfect for travel enthusiasts planning their next adventure.
Features

Search Destinations: Enter a city name (e.g., Paris, Tokyo, New York) to fetch real-time weather data, stunning visuals, and a brief summary of the destination.
Interactive Destination Cards: View beautifully designed cards with city images, weather details (temperature, description, and icons), and a brief description. Each card supports hover effects and removal options.
Modal with Gallery: Click a card to open a modal showcasing a curated gallery of images (landmarks, culture, architecture) and a Wikipedia summary for deeper insights.
Local Storage: Save your favorite destinations locally to revisit them anytime, with options to remove individual destinations or clear all.
Responsive Design: Fully responsive layout with mobile-friendly search and grid views, ensuring a seamless experience across devices.
Animated Background: A gradient-shifting background with twinkling stars creates an engaging, immersive atmosphere.
Error Handling: User-friendly error messages for invalid inputs or API issues, with a 5-second auto-dismiss feature.

Technologies Used

Frontend: HTML5, CSS3, JavaScript (Vanilla)
APIs:
OpenWeatherMap: Fetches real-time weather data for searched cities.
Unsplash: Provides high-quality city images and curated galleries.
Wikipedia REST API: Retrieves summaries for destinations.


Fonts: Poppins (via Google Fonts) for a modern, clean typography.
Local Storage: Persists user-selected destinations across sessions.
CSS Features: Glassmorphism, CSS animations, gradients, and media queries for responsiveness.

Getting Started
Prerequisites

A modern web browser (e.g., Chrome, Firefox, Edge).
An active internet connection for API requests.
API keys for OpenWeatherMap and Unsplash (optional for custom keys, as demo keys are included).

Installation

Clone the Repository:
git clone https://github.com/your-username/wander-explorer.git
cd wander-explorer


Get API Keys (Optional):

OpenWeatherMap: Sign up at openweathermap.org to get a free API key. Replace the demo key in index.html (line ~330) with your own:const OPENWEATHER_API_KEY = 'your-openweather-api-key';


Unsplash: Sign up at unsplash.com/developers for a free API key (50 requests/hour in demo mode). Replace the demo key in index.html (line ~328):const UNSPLASH_ACCESS_KEY = 'your-unsplash-access-key';



Note: The included demo keys work for testing but have rate limits. Using your own keys is recommended for production or heavy usage.

Serve the Application:

Since this is a static HTML file with client-side JavaScript, you need a local server to handle API requests (due to CORS restrictions).
Option 1: Use a local development server like live-server:npm install -g live-server
live-server


Option 2: Use Python’s HTTP server:python3 -m http.server 8000


Open your browser and navigate to http://localhost:8000 (or the port provided by the server).


Explore:

Enter a city name in the search bar (e.g., “Paris” or “Tokyo”) and press “Explore Now” or hit Enter.
View destination cards, click to see details in a modal, or remove destinations as needed.



File Structure
wander-explorer/
├── index.html         # Main HTML file with embedded CSS and JavaScript
├── README.md          # Project documentation (this file)

Usage

Search for a Destination:

Type a city name in the search bar and click “Explore Now” or press Enter.
The app fetches weather data, a main image, and a gallery of related images, displaying them in a card.


Interact with Cards:

Hover over a card for a smooth scale and shadow effect.
Click a card to open a modal with a gallery and summary.
Click the × button on a card to remove it from your list.


Manage Destinations:

Use the “Clear All” button to remove all saved destinations (with a confirmation prompt).
Destinations are saved in the browser’s localStorage for persistence.


View on Mobile:

The layout adjusts automatically for smaller screens, with a stacked search bar and single-column grid.



Screenshots
Hero Section
<img width="1891" height="862" alt="ss1" src="https://github.com/user-attachments/assets/4e110ff2-30a6-4ba2-a6bd-d42908714811" />

Empty State

<img width="1902" height="867" alt="ss2" src="https://github.com/user-attachments/assets/5c70b636-825c-4058-b2f5-fa803f8aaa81" />
Modal Gallery (Paris)

<img width="1898" height="867" alt="ss3" src="https://github.com/user-attachments/assets/d6abcff6-0356-4362-8cfd-83db191862aa" />
Destination Card (Paris)
<img width="1896" height="857" alt="ss4" src="https://github.com/user-attachments/assets/41919df9-bb39-4562-bb47-a5a53815d8c7" />

Limitations

API Rate Limits: The demo Unsplash key is limited to 50 requests/hour, and the OpenWeatherMap key has usage restrictions. Use personal API keys for extended use.
Security: API keys are hardcoded in the client-side JavaScript, which is not suitable for production. Consider a backend proxy for secure key management.
Image Fallback: If Unsplash returns no images, a default image is used, which may not always be relevant.
Accessibility: Some elements (e.g., gradient text) may need contrast improvements for accessibility.

Future Improvements

Backend Integration: Move API keys to a server-side proxy (e.g., Node.js/Express or Flask) for security.
Caching: Store API responses in localStorage to reduce redundant calls and handle rate limits.
Debouncing: Add debouncing to the search input to prevent rapid API requests.
Sorting/Filtering: Allow users to sort destinations by temperature or name, or filter by country.
Accessibility: Enhance ARIA attributes and text contrast for better accessibility.
Offline Support: Implement a service worker to cache static assets for offline access.

Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch (git checkout -b feature/your-feature).
Make your changes and commit (git commit -m "Add your feature").
Push to the branch (git push origin feature/your-feature).
Open a pull request with a clear description of your changes.

Please ensure your code follows the existing style and includes comments for clarity.
License
This project is licensed under the MIT License. Feel free to use, modify, and distribute the code as per the license terms.
Acknowledgements

OpenWeatherMap for weather data.
Unsplash for stunning city images.
Wikipedia for city summaries.
Poppins Font for beautiful typography.

Contact
For questions, suggestions, or feedback, reach out via GitHub Issues or connect with me on LinkedIn.
Happy exploring with WanderExplorer! ✈️🌍
