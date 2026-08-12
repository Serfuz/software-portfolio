# YATZY - Web-Based Local Multiplayer Game

## Overview
This project is a browser-based Yatzy game built as a full-stack web application for a university software engineering assignment. The game is designed as a local hot-seat experience (2-4 players) where users can start new games, continue from saved state, and track highscores.

The application combines server-side user/session handling with client-side game logic. Game state is persisted in browser cookies for all players, and authenticated users can also save and reload games from the database.

## Technologies
- Python
- Flask
- JavaScript (vanilla)
- HTML (Jinja templates)
- CSS
- SQLite
- REST-style JSON API endpoints
- Session cookies
- Werkzeug password hashing

## Team Size
2 computer engineering students.

## Implemented Features
- Login and registration with server-side validation.
- Password hashing and authenticated session handling.
- Yatzy gameplay in the browser with dice rolling and scoring logic.
- New game flow for 2-4 players.
- Save, load, update, and delete game saves for logged-in users.
- Highscore list with automatic update when games are finished.
- Frontend form validation and user feedback for invalid input.
- Responsive layout adjustments for smaller screens.

## Architecture and Structure
- Flask app entry point in `YATZY/app.py` with route handlers and validation logic.
- Database access and SQL operations separated into `YATZY/db_functions.py`.
- Frontend behavior split across `YATZY/static/script.js` (UI/auth/panels) and `YATZY/static/board.js` (game logic).
- UI composed with reusable templates in `YATZY/templates/`.

## What This Project Demonstrates
- Building a complete CRUD-capable web app with authentication.
- Combining client-side interactivity with server-side persistence.
- Designing and using REST-like endpoints with meaningful HTTP status codes.
- Structuring a student project with clear separation of backend, database, and frontend responsibilities.
