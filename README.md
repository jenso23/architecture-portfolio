How It Works (Architecture & Dynamic Fetching)
Centralized Data Management (content.json)

All dynamic content (personal details, project descriptions, image paths, metadata, and navigation links) is stored in a single content.json file.

Updating project text, adding new images, or modifying CV entries only requires editing content.json, leaving the HTML markup untouched.

Asynchronous Data Rendering (fetch API)

Each page uses native JavaScript (fetch('content.json')) to asynchronously retrieve the latest content upon loading.

The JavaScript dynamically populates the DOM elements, rendering project galleries, metadata grids, narrative sections, and navigation menus on the fly.

Interactive Features

Fullscreen Snap Slider (index.html): CSS Scroll Snap paired with dynamic JavaScript controls for quick dot navigation and dropdown linking.

Interactive Image Lightbox: Modal gallery viewer with smooth click-to-zoom and cursor-following panning functionality for viewing detailed architectural drawings and site plans.

Deployment
This website is automatically deployed using GitHub Pages.

Hosting Source: Main branch

Path Resolution: Relative file paths without leading slashes (ensuring strict case-sensitivity compatibility across Linux-based web servers).

Built With
HTML5 & CSS3 (Custom Properties, Flexbox, CSS Grid, Scroll Snap)

Vanilla JavaScript (ES6+) (Fetch API, DOM Manipulation)

Google Fonts (Cinzel for headings, Plus Jakarta Sans for modern body typography)
