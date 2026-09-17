# Neon Tic-Tac-Toe Ultimate

Play URL: https://joenasriani.github.io/tictactoe-advanced/

A browser-based Tic-Tac-Toe game implemented in a single `index.html` file. It includes a 3D tilt/parallax interface, CPU play, local two-player play, adaptive board expansion after draws, and code for Firebase-backed online rooms.

## Run locally

Open `index.html` in a modern browser. The CPU and local two-player modes do not require a build step or local server.

## Gameplay

- The game starts on a 3x3 board.
- A draw expands the next round to 4x4, then 5x5 and larger boards.
- The win condition scales with the board size: 3 in a row on 3x3, 4 in a row on 4x4, and so on.
- CPU mode uses Minimax on 3x3 boards and simpler move-selection logic on larger boards.
- Local mode supports two players on the same device.
- Online mode contains Firebase Authentication and Firestore room logic.

## Interface

- Mouse and touch position drive the board tilt effect.
- Board elements use layered transforms and parallax-style depth.
- The layout adapts to mobile viewport dimensions.
- The board scales to the available screen area.

## Technology

- HTML5
- Vanilla JavaScript (ES modules)
- Tailwind CSS loaded from CDN
- Google Fonts loaded from CDN
- Firebase Authentication and Firestore modules loaded from CDN

## Online mode configuration

The current source expects Firebase-related globals to be supplied at runtime:

- `__app_id`
- `__firebase_config`
- optional `__initial_auth_token`

If `__firebase_config` is not supplied, the code falls back to an empty configuration object and Firebase initialization cannot provide a working online session. The GitHub Pages URL by itself does not inject these values.

## Controls

- Mouse: move the pointer to tilt the board; click a cell to place a mark.
- Touch: tap a cell to place a mark; touch movement also affects the tilt position.

## Repository status

This repository contains `README.md` and `index.html`. No separate `LICENSE` file is currently included, so the repository should not be treated as having an explicit repository-level license solely from the previous README wording.
