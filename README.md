
>> https://joenasriani.github.io/tictactoe-advanced/

Neon Tic-Tac-Toe Ultimate
A futuristic, high-performance Tic-Tac-Toe game built with modern web technologies. This project features a holographic 3D interface, intelligent AI, and real-time online multiplayer capabilities, all contained within a single responsive file.
PLAY THE GAME
Simply open the index.html file in any modern web browser. No build steps, installation, or local server are required.
FEATURES
 * Immersive 3D Experience
   * Holographic Tilt Effect: The board rotates and shifts perspective based on mouse movement (desktop) or gyroscope/touch (mobile).
   * Depth Layers: UI elements, the board, and markers (X/O) float at different Z-indexes for a parallax effect.
   * Glassmorphism: Frosted glass panels with dynamic lighting and blur effects.
 * Adaptive Gameplay
   * Dynamic Grid Expansion: The game evolves from 3x3 to 4x4, 5x5, and beyond if a match ends in a draw.
   * Scaling Win Conditions: Win logic adapts automatically (3-in-a-row for 3x3, 4-in-a-row for 4x4, etc.).
   * Smart CPU: An AI opponent that uses Minimax for small grids and advanced heuristics for larger boards to ensure performance.
 * Game Modes
   * vs CPU: Challenge the adaptive AI.
   * Local PvP: Play against a friend on the same device.
   * Online Multiplayer: Real-time matchmaking using Firebase. Create a room, share the code, and play across devices.
 * Mobile-First Design
   * Responsive Layout: Dynamic Viewport Height (dvh) support ensures perfect fit on all mobile browsers.
   * Touch Optimization: Optimized for tap targets and swipe prevention.
   * Flexible Grid: Board scaling ensures playability on screens of all sizes.
TECH STACK
 * Core: HTML5, Vanilla JavaScript (ES6+)
 * Styling: Tailwind CSS (via CDN)
 * Backend: Firebase Firestore & Authentication (v11.6.1)
 * Fonts: Orbitron (Headers) & Inter (UI)
CONFIGURATION
The game connects to Firebase for multiplayer functionality. The configuration is handled via global variables injected at runtime or can be manually set in the script tag within index.html.
Controls
 * Mouse: Move cursor to tilt the board; Click to place mark.
 * Touch: Tap to place mark; Drag slightly to tilt perspective.
License
This project is open source and available under the MIT License.
