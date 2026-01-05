# Project Overview

**Ethan's Arcade** is a personal portfolio and landing page designed with a retro arcade aesthetic. It serves as a creative showcase for games and other projects. The interface mimics an arcade cabinet, where users can browse and launch different games.

**Key Features:**
*   **Retro UI:** styled with a pixel-art arcade cabinet background and the "Press Start 2P" font.
*   **Interactive Cabinet:** The layout is positioned to fit within the screen area of the arcade cabinet image.
*   **Game Launcher:** Buttons on the arcade screen allow users to launch hosted games (currently configured to open in new tabs).

# Technology Stack

*   **HTML5:** Semantic structure for the application.
*   **CSS3:** Embedded styles for layout, animations, and responsiveness. Handles the positioning of the "screen" within the cabinet image.
*   **JavaScript:** Vanilla JS for handling user interactions (clicking games).

# Directory Structure

*   **`index.html`**: The core file containing all HTML, CSS, and JavaScript. This is the entry point for the website.
*   **`WorkingBackground.png`**: The main background image depicting the arcade cabinet.
*   **`*.aseprite`**: Source files for the pixel art graphics, created using Aseprite. These are the editable source files for the PNGs.
*   **`FinalArcadeBackground-*.png`**: Various exported states of the arcade background (likely for animations or different interaction states like button presses or joystick movements).
*   **`resume.pdf`**: A PDF resume file.

# Setup and Usage

## Running the Project
Since this is a static website, you do not need a build process.
1.  **Local:** Simply open `index.html` in any modern web browser.
2.  **Hosting:** This project is configured for GitHub Pages (indicated by the `akiyamaethan.github.io` directory name). Committing changes to the `main` (or `master`) branch will automatically update the live site.

## Development Notes
*   **Adding Games:** To add a new game, duplicate one of the `.game-thumb` divs in `index.html` and update the `onclick` handler with the game's name and URL.
*   **Styling:** All styles are currently located in the `<style>` block within `index.html`.
*   **Assets:** When modifying the arcade cabinet graphics, edit the `.aseprite` files and export them to PNG. Ensure the screen area coordinates in the CSS (`.screen-area`) match any changes to the background image.

## Current Behavior vs. Code Structure
The JavaScript implementation (`openGame` function) opens links in a new tab. Previous experimental functionality for inline iframes has been removed to streamline the experience.
