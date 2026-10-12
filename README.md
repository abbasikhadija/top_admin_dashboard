Admin Dashboard
A desktop-focused dashboard interface built with HTML and CSS. The design combines a dark theme, neon pink accents, project cards, and a persistent sidebar using nested CSS Grid layouts and Flexbox.
Created as part of The Odin Project to practise building a complete dashboard layout without a CSS framework.
Interface Features
- Sticky sidebar with navigation labels, inline SVG icons, and a lower settings section.
- Two-row header with a search field, profile details, greeting, and action buttons.
- Six project cards arranged in a two-column grid.
- Announcements panel with separated entries.
- Trending panel with user avatars and project names.
- Shared CSS custom properties for colors, spacing, border radius, and shadows.
- Locally loaded custom font with system-font fallbacks.
- Hover feedback on the New, Upload, and Share buttons.
Project Scope
This is a static interface project. Search, navigation, project actions, and the New, Upload, and Share buttons are visual elements without application logic. Project descriptions and announcements are sample content, not implemented services or features. No JavaScript, backend, authentication, or data storage is included.
Technologies
Technology	Purpose
HTML5	Dashboard structure and content
CSS Grid	Page layout, main content columns, project grid, and panel alignment
Flexbox	Sidebar arrangement, card content, profile details, and button groups
CSS custom properties	Centralized theme and spacing values
Inline SVG	Navigation and action icons embedded in the HTML
@font-face	Loading local WOFF2 and WOFF font files


Layout Approach
The page uses a 260px sidebar beside the main dashboard area. Inside the dashboard, the header sits above a second grid that separates project cards from announcements and trending content. The project section uses its own two-column grid.
Flexbox handles smaller groups within these regions, including profile information, action buttons, and the vertical arrangement of card content. Keeping theme values in :root makes it easier to adjust the visual style consistently.
Run Locally
Download or clone the repository and open the HTML entry file in your browser. If creating the project from the source, save the HTML as index.html and the CSS as style.css.
Keep these assets at the paths referenced by the code:
Path	Purpose
index.html	Dashboard markup
style.css	Dashboard styling
geofont-edge-bold-webfont.woff2	Primary custom font file
geofont-edge-bold-webfont.woff	Alternative custom font format
svgs/dp.jpeg	Main profile image
svgs/liam.jpeg	Trending avatar
svgs/emma.jpeg	Trending avatar
svgs/sophia.jpeg	Trending avatar
svgs/noah.jpeg	Trending avatar


No package installation or build step is required. If the font files are unavailable, the browser uses the specified fallback fonts. Image files must be supplied separately.
Current Limitations
- The layout has no mobile breakpoints and may overflow on smaller screens.
- Controls and navigation do not yet perform actions.
- Accessibility needs further work, including semantic navigation, a search label, descriptive image alternatives where appropriate, and visible keyboard focus styles.
Planned Improvements
- Add tablet and mobile layouts with a collapsible sidebar and a single-column project grid.
- Implement project filtering and task interactions with JavaScript.
- Improve semantic HTML and keyboard accessibility.
- Consolidate duplicate CSS rules and standardize SVG markup.
Concepts Practised
Nested grids, one-dimensional alignment with Flexbox, reusable styling, sticky positioning, local font loading, inline SVG integration, and visual hierarchy.
